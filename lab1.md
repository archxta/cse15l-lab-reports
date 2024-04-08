# lab 1
## cd command
1. **no args**

Absolute path before running command: /Users/architap
```
  architap@Architas-MacBook-Pro ~ % cd
  architap@Architas-MacBook-Pro ~ % 
```
The command cd with no args brought me back to the home directory, and since my current working directory was already at home, this command does not change the directory. This output is not an error. 

2. **path to directory as argument**

Absolute path before running command: /Users/architap
```
architap@Architas-MacBook-Pro ~ % cd cse15l-lab-reports/
architap@Architas-MacBook-Pro cse15l-lab-reports % 

```
The command cd with a path to the cse15l-lab-reports directory brought me back to the cse15l-lab-reports directory as shown above. Thus, the current directory changed from home to cse15l-lab-reports after running this command. This output is not an error. 

3.  **path to file as argument**

Absolute path before running command: /Users/architap/cse15l-lab-reports
```
architap@Architas-MacBook-Pro cse15l-lab-reports % cd sample.md
cd: not a directory: sample.md
architap@Architas-MacBook-Pro cse15l-lab-reports % 

```
The command cd with a path to the sample.md file inside the cse15l-lab-reports directory produced an error since we cannot change our directory to a file. We can only set our directory to another directory and not another file.  

## ls command
1. **no args**

Absolute path before running command: /Users/architap
```
architap@Architas-MacBook-Pro ~ % ls
Applications		Documents		Pictures
CSE 12			Downloads		Public
CSE 12 PAs		Library			cse15l-lab-reports
CSE 12.code-workspace	Movies			detective.json
Desktop			Music			lecture1

```
The command ls with no args produced a list of all the directories inside the architap directory (my current directory) which are the directories shown above. This output is not an error. 

2. **path to directory as argument**

Absolute path before running command: /Users/architap
```
architap@Architas-MacBook-Pro ~ % ls cse15l-lab-reports
index.md	lab1.md		sample.md

```
Before running this commmand, I am still in my home directory (/Users/architap). The command ls with a path to the cse15l-lab-reports directory displayed all the files inside the cse15l-lab-reports directory. This output is not an error. 

3. **path to file as argument**

Absolute path before running command: /Users/architap
```
architap@Architas-MacBook-Pro ~ % ls cse15l-lab-reports
index.md	lab1.md		sample.md
architap@Architas-MacBook-Pro ~ % ls cse15l-lab-reports/sample.md
cse15l-lab-reports/sample.md

```
Before running this commmand, I am still in my home directory (/Users/architap) since I did not change the directory at any point. The command ls with a path to the file sample.md simply displays the path to the file. This is not an error, but this command can't display the contents of the file so it merely outputs the path to this file as seen above. 

## cat command
1. **no args**

Absolute path before running command: /Users/architap
```
  architap@Architas-MacBook-Pro ~ % cat
  hi
  hi
  this command copies everything i input
  this command copies everything i input
  ^C 
```
If you run the cat command with no arguments, it will wait for input from the keyboard and after you type some input and press Enter, it will display that input back to you. As seen above, when I typed hi, it displayed hi back to me. To exit the cat command, you have to press control c and this is represented by ^C in the terminal. This does not produce an error, but the terminal is waiting for a file name that follows the cat command. 

2. **path to directory as argument**

Absolute path before running command: /Users/architap
```
architap@Architas-MacBook-Pro ~ % cat cse15l-lab-reports
cat: cse15l-lab-reports: Is a directory

```
The command cat with a path to the cse15l-lab-reports directory  outputs an error message indicating that cse15l-lab-reports is a directory and not a file. The cat command expects files as arguments so it can display the contents of the file, so attempting to use it with a directory will result in this error. 

3. **path to file as argument**

Absolute path before running command: /Users/architap
```
architap@Architas-MacBook-Pro ~ % cat cse15l-lab-reports/sample.md
this is a sample file

```
The command cat with a path to the cse15l-lab-reports/sample.md file outputs the contents inside the sample.md file (this is a sample file). The cat command expects files as arguments so with a file argument, it concatenates the contents of the file and outputs them directly to the terminal. 










   













