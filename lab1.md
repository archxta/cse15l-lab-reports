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

##cat command
1. **no args**

Absolute path before running command: /Users/architap
```
  architap@Architas-MacBook-Pro ~ % cd
  architap@Architas-MacBook-Pro ~ % 
```
The command cd with no args brought me back to the home directory, and since my current working directory was already at home, this command does not change the directory. This output is not an error. 





   













