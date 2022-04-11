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
  <summary>» This is a spoiler, Click Me!</summary>
  This is the inside of a spoiler where images will be located!
  </details>

On with it then!

---

## Part 1 - Installing VSCode
1. Visit the VSCode website (https://code.visualstudio.com/) and click the download button for your respective operating system.

<details>
  <summary>» Download Button</summary>
  
  <img src="lab1images/vscodedownloadbutton.png" alt="VSCode Download Button"></img>
  
</details><br />
  
2. Run the installer if necessary, or if you downloaded a zip file, just unarchive that and drag VSCode to your Applications Folder.
3. Open VSCode. You should be greeted with a window that looks something like this!

<details>
  <summary>» VSCode Window</summary>
  
  <img src="lab1images/vscodewindow.png" alt="VSCode Window"></img>
  
  </details>

That is all for Part 1! You now have VSCode downloaded and installed.

## Part 2 - Remotely Connecting into the ```ieng6``` server at UCSD.
To connect to the remote server named ```ieng6``` at UCSD, we will be using the SSH command.

1. At the bottom of your VSCode window, you should see a section labled *Terminal*.

<details>
  <summary>» VSCode Terminal</summary>
  
  <img src="lab1images/vscodeterminal.png" alt="VSCode Terminal"></img>
  
</details><br />
  
2. In that terminal section, enter the command ```ssh username@ieng6.ucsd.edu```
  - ```ssh``` Is the command being run.
  - ```username``` Refers to your course-specific account username. It most likely starts with ``cs15l``. Enter your unique username here.
  - ```@ieng6.ucsd.edu``` Tells your computer where to connect to. In this case, it is the ```ieng6``` server at UCSD.
3. Once you press enter, you will be asked if you are sure that you want to continue connecting with a (yes/no) prompt. Enter ```yes``` and press enter to save the ```ieng6``` server as a known host on your computer.
4. Next, you will be asked for a password. Enter your course-specific account password here.
  - You will not see your password being entered as you type it! Do not worry, this is normal. It is a security feature.
  - Make sure you entered/pasted your password correctly, then press enter.
5. At this point, you have successfully connected to the ```ieng6``` server! You should be greeted with messages that look something like this.

<details>
  <summary>» Welcome Messages</summary>
  
  <img src="lab1images/welcomemessages.png" alt="Welcome Messages"></img>
  
</details><br />
  
  
