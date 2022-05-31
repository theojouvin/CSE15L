## Lab Report 4
### Testing the Implementation of Two Versions of MarkdownParse
---

This lab report contains the following;
- A link to my lab group's Markdown Parser repository.
- A link to another lab group's Markdown Parser repository that my group reviewed.
- For three Markdown code snippets:
  - Expected Output
  - MarkdownParseTest Code
  - Test results for both implementations of MarkdownParse
  - Potential code fixes to achieve expected output, if necessary.

Screenshots will be included in spoilers as to not take up uncessary space. 

<details>
  <summary> » This is a spoiler, Click Me!</summary>
  This is the inside of a spoiler where images will be located!
  </details>

---

My lab group's Markdown Parser repository: https://github.com/Mashyuf/markdown-parser
The reviewed Markdown Parser repository: https://github.com/cmy0357/markdown-parser

---

## 1. Snippet 1

  Using SSH Keys instead of a password made connecting to the remote server easier. Adding the host to the ```/.ssh/config``` file makes the process of remote connecting even faster. I added a few lines shown in the first image into the config file using TextEdit. Then, in the second image, I demonstrated logging in with the ```ssh``` command using the nickname that I gave the host in the config file. Finally, in the last image, I demonstrated copying a file over to the remote server using the ```scp``` command. This was all much faster and easier!
  
<details>
  <summary> » SSH Configuration File</summary>
  <img src="lab3images/sshconfig.gif" alt="SSH Configuration File">
  </details>

<details>
  <summary> » Quickly Logging in to Remote Server Using SSH Command</summary>
  <img src="lab3images/sshlogin.gif" alt="SSH Login">
  </details>

<details>
  <summary> » Quickly Copying a File Using SCP Command</summary>
  <img src="lab3images/scp.gif" alt="SCP">
  </details>


## 2. Snippet 2

  Cloning a GitHub Repository to the remote server using its link only allows limited access to the repository. (Ex. Checking the status and pulling updates). If we want to commit and push changes, further authentication needs to be set-up. I went through this process, and created SSH keys to do so. Shown in the first spoiler are the locations of the public key (```~/.ssh```) on the remote server and on GitHub. Shown in the second spoiler is the location of the private key on the remote server (also in the ```~/.ssh``` folder). In the third spoiler, I staged, committed, and pushed a change to GitHub. Lastly, the fourth spoiler and accompanying link shows the commit.
  
<details>
  <summary> » Public Key Location</summary>
  <img src="lab3images/ieng6GHPubKey.png" alt="Public Key on Remote Server">
  <img src="lab3images/GHPubKey.png" alt="Public Key on GitHub">
  </details>

<details>
  <summary> » Private Key Location</summary>
  <img src="lab3images/ieng6GHPrivKey.png" alt="Private Key on Remote Server">
  </details>
  
  <details>
  <summary> » GitHub Commands on Remote Server</summary>
  <img src="lab3images/ieng6GHCommands.png" alt="GitHub Commands on Remote Server">
  </details>
  
  <details>
  <summary> » GitHub Commit Log + Link</summary>
  <img src="lab3images/ieng6Commit.png" alt="Commit from Remote Server">
  <a href="https://github.com/theojouvin/CSE15L/commit/bbdbf48de7ca5cbd56ee5ff50e299556e606265a" target="_blank">Commit from Remote Server</a>
  </details>
  
  
## 3. Snippet 3

  Copying an entire folder to a remote server is as easy as adding the ```-r``` flag to the ```scp``` command. In the first image, I demonstrate copying the entirety of the MarkdownParse folder. In the second image, I compiled and ran tests on the remote server in the directory that I had just copied over. In the last image, I demonstrated copying a directory, compiling, and running tests, all in one command using quotes and semi-colons.
  
<details>
  <summary> » Copying an Entire Directory</summary>
  <img src="lab3images/copywholedir.gif" alt="Copying an Entire Directory">
  </details>

<details>
  <summary> » Testing on the Remote Server Using Copied Directory</summary>
  <img src="lab3images/testcopieddir.gif" alt="Testing with Copied Directory">
  </details>

<details>
  <summary> » Copying an Entire Directory and Testing in One Command</summary>
  <img src="lab3images/combinecmds.gif" alt="Combining Commands">
  </details>
