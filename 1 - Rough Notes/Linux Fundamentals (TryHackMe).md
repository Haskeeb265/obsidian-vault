
2025-01-25 12:29

Status: #InProgress

Tags: [[linux]] [[cybersecurity]] 

# Linux Fundamentals (TryHackMe)

Linux is used in almost every commercial application such as:
1. Home appliances
2. Traffic lights
3. Web servers and more

- Linux is very lightweight. It can run on a system with only 512MB RAM. 
- Linux is actually an umbrella term for multiple OS's
- Linux is open source and thanks to that we can all the OS's that are developed for different use cases.
- The first Linux distribution was released in 1991

### Ubuntu Commands:
1. echo "Message": Outputs the message
2. whoami: Shows who you're logged in as
3. ls: Lists all the directories in the current directory or desktop that you're in. To list the items within the directories, you can you use ==ls "directory name"== this way you would've have to go into each directory to see its contents
4. cd "name of directory": Changes the directory that we are in.
5. cd .. : Goes back to the previous directory
6. cat: Cat stands for concatenate. We use this command to give us an output of files.
7. pwd: pwd stands for **Print Working Directory** this command is used to keep track of where you are in the filesystem.
8. find -name *name of file*: The find command helps us search for files through the entire system. Instead of using ls, cd, repeatedly for all available directories, we can run a single find command and it will return the path of the file that we're looking for.
    Let's say you don't know the name of the file that you're looking for. What you can do is use **wildcard**  * is a wild card. With the help of * we can specify the filetype that we're looking for. For example:
	    find -name *.txt
	    The above command would return every file which holds the extension .txt in the end.

9. grep: This command is used to find a specific value within a file. Consider a file with 100 names and you want to find the name "Haseeb". Instead of going through the entire file. For example, grep "Haseeb" names.txt would fetch the name Haseeb from names.txt if it exists.



#### References
[[Linux Fundamentals]]