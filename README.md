In this project, we explore how to effectively use Standard Output (stdout) and Standard Error (stderr) in Linux to handle the output of commands and errors in a real-world situation.
<h1> standard-error-and-output-in-Linux</h1>


<h2>Description</h2>
In this project, we explore how to effectively use Standard Output (stdout) and Standard Error (stderr) in Linux to handle the output of commands and errors in a real-world situation.


<h2>Task: Your boss has asked you to find all the .log and .txt files across the entire filesystem, including the ones you don't have access to. To do this, you'll need to create two files:

One file that lists all the files you have access to.

Another file that lists all the files you don't have access to (permission denied).

 </h2>

- <b>Linux Ubuntu</b>

 <h2>Real World Problem:</h2>
Imagine you work as an IT support specialist, and a customer needs you to create a directory named 'school' to organize their school work, divided into subdirectories for each class. The customer also wants you to remove their old 'school' directory and create a symbolic link named '123' to the new 'school' directory.
<br />


<h2>walk-through:</h2>


<p align="center">
<br />
<br />
Once you're in the terminal, you can check which directory you're in by typing the command "pwd". To store the user files, you can do this in the /home/username directory. If you're not there already, you can navigate to it by typing the command "cd /home/username".: <br/>
 <img src="<a href="https://ibb.co/F4sRdnd8"><img src="https://i.ibb.co/r2bDXvX5/Screenshot-2025-03-16-133632.png"  height="80%" width="80%" alt="steps"/>
<br />
<br />
To list all the directories located in /home/username, you will need to type the command "ls -l". After doing this, we will see that the directory 'school' already exists, and this is the directory the customer wants us to remove.":  <br/>
<img src="<a href="https://ibb.co/1fhF06kN"><img src="https://i.ibb.co/BVd0fN9J/Screenshot-2025-03-16-134424.png" height="80%" width="80%" 
<br />
<br />
To remove the old 'school' directory along with its contents, we will use the command "rm -r school". To check that the directory has been removed, we can use the "ls -l" command.: <br/>
<img src="<a href="https://imgbb.com/"><img src="https://i.ibb.co/yDyFgCk/Screenshot-2025-03-16-134810.png" height="80%" width="80%"
<br />
<br />
To create a new directory, we will use the command "mkdir school".:  <br/>
<img src="<a href="https://ibb.co/svfyKy9H"><img src="https://i.ibb.co/8DC6r6gc/Screenshot-2025-03-16-135255.png" height="80%" width="80%" 
<br />
<br />
:  <br/>
To grant the user read, write, and execute permissions, we will use the command "chmod u=rwx school". To check the permissions, we will run the command "ls -ld school".:  <br/>
<img src="<a href="https://ibb.co/j9vfS6gy"><img src="https://i.ibb.co/1YfQkv8r/Screenshot-2025-03-16-140843.png" height="80%" width="80%"
<br />
<br />
Now, to create a subdirectory for each of his classes, we will use the command mkdir -p school/class. We will do this for both his science and math classes.:  <br/>
<img src="<a href="https://ibb.co/VYRWb4vV"><img src="https://i.ibb.co/SwbXHCKN/Screenshot-2025-03-16-142020.png" height="80%" width="80%" 
<br />
<br />
To create a symbolic link, we will use the command "ln -s school 123".:  <br/>
<img src="<a href="https://ibb.co/cKGZmwfN"><img src="https://i.ibb.co/6c3Td894/Screenshot-2025-03-16-143321.png" height="80%" width="80%"      

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
