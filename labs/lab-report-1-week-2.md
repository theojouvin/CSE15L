## Lab Report 1
### Logging Into and Using Your Course Specific Account on ```ieng6``` at UCSD.
---

Hello new and incoming 15L students! In this guide, you will learn the following:
- Installing VSCode
- Remotely connecting into the ```ieng6``` server at UCSD
- Basic Linux/Command Prompt Commands
- Moving files between a client & server
- Setting up an SSH Key
- Optimizing remote running

This guide will be formatted into multiple parts with explanations and screenshots of different steps. Screenshots will be included in spoilers as to not take up uncessary space. 
<details>
  <summary> » This is a spoiler, Click Me!</summary>
  This is the inside of a spoiler where images will be located!
  </details>

On with it then!

---

## Part 1 - Installing VSCode
1. Visit the VSCode website ([https://code.visualstudio.com/](https://code.visualstudio.com/)) and click the download button for your respective operating system. 
2. Run the installer if necessary, or if you downloaded a zip file, just unarchive that and drag VSCode to your Applications Folder.
3. Open VSCode. You should be greeted with a window that looks something like this!

<details>
  <summary> » Download Button</summary>
  
  <img src="lab1images/vscodedownloadbutton.png" alt="VSCode Download Button">
  
</details> 
<details>
  <summary> » VSCode Window</summary>
  
  <img src="lab1images/vscodewindow.png" alt="VSCode Window">
  
  </details>  

That is all for Part 1! You now have VSCode downloaded and installed.

## Part 2 - Remotely Connecting into the ```ieng6``` server at UCSD.
To connect to the remote server named ```ieng6``` at UCSD, we will be using the SSH command.

1. At the bottom of your VSCode window, you should see a section labled *Terminal*.
2. In that terminal section, enter the command ```ssh username@ieng6.ucsd.edu```
  - ```ssh``` Is the command being run.
  - ```username``` Refers to your course-specific account username. It most likely starts with ``cs15l``. Enter your unique username here.
  - ```@ieng6.ucsd.edu``` Tells your computer where to connect to. In this case, it is the ```ieng6``` server at UCSD.
3. Once you press enter, you will be asked if you are sure that you want to continue connecting with a (yes/no) prompt. Enter ```yes``` and press enter to save the ```ieng6``` server as a known host on your computer.
4. Next, you will be asked for a password. Enter your course-specific account password here.
  - You will not see your password being entered as you type it! Do not worry, this is normal. It is a security feature.
  - Make sure you entered/pasted your password correctly, then press enter.
5. At this point, you have successfully connected to the ```ieng6``` server! You should be greeted with some welcome messages telling you the following:
  - Which specific server you are connected to.
  - How much of the CPU you are currently using.
  - Usage averages across other servers.
  - The date and time.

<details>
  <summary> » VSCode Terminal</summary>
  
  <img src="lab1images/vscodeterminal.png" alt="VSCode Terminal">
  
</details>  
<details>
  <summary> » Welcome Messages</summary>
  
  <img src="lab1images/welcomemessages.png" alt="Welcome Messages">
  
</details>  
  
That is all for Part 2! You have now successfully connected to the ```ieng6``` server.

## Part 3 - Basic Linux/Command Prompt Commands
We will now go over some basic commands that are useful to know. As you go through this guide, try these commands yourself and see if you get the same outputs!

1. ```cd <directory>``` Try "/"
  - The ```cd``` command can move you to different directories. In this case, with "/" you will be moved to the root directory of the server.
2. ```cd``` or ```cd ~```
  - Using the ```cd``` command with no arguments or with the "~" symbol will bring you to your home directory.
3. ```pwd```
  - This command will print the current working directory.
4. ```ls```
  - This command will list all of the files in your current directory.
5. ```ls -l```
  - The ```ls``` command with the "-l" argument will list all of the files in your current directory vertically, with in more detail.
6. ```ls <directory>``` Try "/"
  - The ```ls``` command with "/" or any other directory for that matter will list files in that requested directory, even if you are not in it.
7. ```cp /home/linux/ieng6/cs15lxxxx/public/hello.txt ~/```
  - The ```cp``` command will copy a file from one directory to another. Typing it as provided above (with the exception of changing "xxxx" to your current quarter and year) will copy the hello.txt file into your home directory.
8. ```cat /home/linux/ieng6/cs15lxxxx/public/hello.txt```
  - The ```cat``` command will display the contents of file. Typing it as provided above (with the exception of changing "xxxx" to your current quarter and year) will display the contents of hello.txt.

<details>
  <summary> » Command 1</summary>
  
  <img src="lab1images/command1.png" alt="Command 1">
  
</details>  
<details>
  <summary> » Command 2</summary>
  
  <img src="lab1images/command2.png" alt="Command 2">
  
</details>  
<details>
  <summary> » Command 3</summary>
  
  <img src="lab1images/command3.png" alt="Command 3">
  
</details>  
<details>
  <summary> » Command 4</summary>
  
  <img src="lab1images/command4.png" alt="Command 4">
  
</details>  
<details>
  <summary> » Command 5</summary>
  
  <img src="lab1images/command5.png" alt="Command 5">
  
</details>  
<details>
  <summary> » Command 6</summary>
  
  <img src="lab1images/command6.png" alt="Command 6">
  
</details>  
<details>
  <summary> » Command 7</summary>
  
  <img src="lab1images/command7.png" alt="Command 7">
  
</details>  
<details>
  <summary> » Command 8</summary>
  
  <img src="lab1images/command8.png" alt="Command 8">
  
</details>  

That is all for Part 3! You now know a few basic commands.

## Part 4 - 
