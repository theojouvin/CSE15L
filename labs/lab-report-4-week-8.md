
Skip to content
Pull requests
Issues
Marketplace
Explore
@theojouvin
theojouvin /
CSE15L
Public
forked from pages-themes/cayman

Code
Issues
Pull requests
Actions
Projects
Security
Insights

    Settings

CSE15L/labs/
in
master

1

## Lab Report 3

2

### SSH Config, GitHub Access, and Copying Whole Directories

3

---

4

​

5

This lab report contains the following;

6

- An example of an SSH Configuration file making it easier to connect to and transfer files to an external server.

7

- An example of setting up access to GitHub from an external server to allow for remote edits and commits.

8

- An example of copying a whole directory to an external server and running tests with those files.

9

​

10

Screenshots / GIFs will be included in spoilers as to not take up uncessary space. 

11

​

12

<details>

13

  <summary> » This is a spoiler, Click Me!</summary>

14

  This is the inside of a spoiler where images will be located!

15

  </details>

16

​

17

---

18

​

19

## 1. Streamlining SSH Configuration

20

​

21

  Using SSH Keys instead of a password made connecting to the remote server easier. Adding the host to the ```/.ssh/config``` file makes the process of remote connecting even faster. I added a few lines shown in the first image into the config file using TextEdit. Then, in the second image, I demonstrated logging in with the ```ssh``` command using the nickname that I gave the host in the config file. Finally, in the last image, I demonstrated copying a file over to the remote server using the ```scp``` command. This was all much faster and easier!

22

  

23

<details>

24

  <summary> » SSH Configuration File</summary>

25

  <img src="lab3images/sshconfig.gif" alt="SSH Configuration File">

26

  </details>

27

​

28

<details>

29

  <summary> » Quickly Logging in to Remote Server Using SSH Command</summary>

30

  <img src="lab3images/sshlogin.gif" alt="SSH Login">

31

  </details>

32

​

33

<details>

34

  <summary> » Quickly Copying a File Using SCP Command</summary>

35

  <img src="lab3images/scp.gif" alt="SCP">

36

  </details>

37

​

38

​

39

## 2. Setting up GitHub Access from ```ieng6```

40

​

41

  Cloning a GitHub Repository to the remote server using its link only allows limited access to the repository. (Ex. Checking the status and pulling updates). If we want to commit and push changes, further authentication needs to be set-up. I went through this process, and created SSH keys to do so. Shown in the first spoiler are the locations of the public key (```~/.ssh```) on the remote server and on GitHub. Shown in the second spoiler is the location of the private key on the remote server (also in the ```~/.ssh``` folder). In the third spoiler, I staged, committed, and pushed a change to GitHub. Lastly, the fourth spoiler and accompanying link shows the commit.

42

  

43

<details>

Attach files by dragging & dropping, selecting or pasting them.
@theojouvin
Commit changes
Commit summary
Optional extended description

Choose which email address to associate with this commit
Commit directly to the master branch.
Create a new branch for this commit and start a pull request. Learn more about pull requests.

    © 2022 GitHub, Inc.

    Terms
    Privacy
    Security
    Status
    Docs
    Contact GitHub
    Pricing
    API
    Training
    Blog
    About

