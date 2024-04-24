# Lab 3
## Part 1
### Web Server Code

```
import java.io.IOException;
import java.net.URI;
import java.util.ArrayList;
import java.util.List;

class Handler implements URLHandler {

    List<String> messages = new ArrayList<>();

    public String handleRequest(URI url) {
       
  
            if (url.getPath().contains("/add-message")) {
                String urlS = url.toString();
                String message = "";
                String user = "";

                if (url.getQuery().contains("s=")) {
                    message = urlS.split("s=")[1];
                    message = message.split("&")[0];
                }

                if (url.getQuery().contains("user=")) {
                    user = urlS.split("user=")[1];
                }

                String resultMessage = String.format("%s: %s", user, message);
                messages.add(resultMessage);

                return String.join("\n", messages);
            }
            return "404 Not Found!";
        
    }
}

class NumberServer {
    public static void main(String[] args) throws IOException {
        if (args.length == 0) {
            System.out.println("Missing port number. For the first argument (port number), try any number between 1024 to 49151.");
            return;
        }



        int port = Integer.parseInt(args[0]);

        Server.start(port, new Handler());
    }
}

```
### Examples Messages using /add

![Example 1](./Message1.png)
