# The following walks you through the steps used to install Visual Studio Code
(This is the default development IDE that I use.  You can use a different one)

1) [Download VScode](https://code.visualstudio.com/)

2) Install VScode with all the default options

![](/images/VScodeInstall_A.png)
![](/images/VScodeInstall_B.png)
![](/images/VScodeInstall_C.png)
![](/images/VScodeInstall_D.png)
![](/images/VScodeInstall_E.png)
![](/images/VScodeInstall_F.png)

3) Install the Extensions you wish.  Click on the "Installed" extensions tab. I installed the following (This changes often):

![](/images/VScodeInstall_G.png)

    - Arduino
    - C/C++
    - Code Spell Checker
    - Data Workspace
    - Dracula Official
    - Git Graph
    - GitLens - Git Supercharged
    - IntelliCode
    - IntelliCode API Usage Examples
    - Jupyter (and the rest that get installed with it)
    - Live Sass Compiler
    - Live Server
    - markdownlint
    - Python (and Pylance gets installed with it)
    - Serial Monitor
    - SQL Bindings
    - SQL Database Projects
    - SQL Server (mssql)
    - vscode-pdf
    - YAML

## How to sync a "project" directory on your hard drive to GitHub.com
### _This is mostly a reminder for myself_
<br>

1) Launch VScode and select "Open Folder..." from the "File" menu
    - We are assuming you have run the the full installation process in this guide
2) Click on the Icon shown in the image below and then click on "Initialize Repository"

![](/images/VScodeGITsetup_A.png)

3) You should see a list of all the files in your directory with a "u" sign next to then.  Click on the "+" sign next to the "Changes" drop down menu.  This will stage all the files to be submitted to your local Git repository.

![](/images/VScodeGITsetup_B.png)

4) All the files should now have an "A" next to them.

![](/images/VScodeGITsetup_C.png)

5) Next, click on the box above the "Staged Changes" drop down and type in something like "Initial commit".  Then click on the check mark above the text box.

![](/images/VScodeGITsetup_D.png)

6) You have officially submitted the entire directory to your local Git repository.  Next, we want to setup the link to the GitHub repository.
    - NOTE:  This assumes that you have setup a new repository on GitHub and have the URL link to it!!

7) Click on the three dots to the right of the "SOURCE CONTROL" tab.  Then go down and select the "Remote" "Add Remote..." option

![](/images/VScodeGITsetup_E.png)

8) Type the URL to the Github repository that you previously setup (and in that process, Github gave you the URL)

![](/images/VScodeGITsetup_F.png)

9) Then enter "origin" int he text box and press Enter
![](/images/VScodeGITsetup_G.png)

10) Next, click on the three dots to the right of the "SOURCE CONTROL" tab and select "Push"

![](/images/VScodeGITsetup_H.png)

11) This window should pop up.  Just click "OK"

![](/images/VScodeGITsetup_I.png)

11)  If this is the first time doing this, you will need to Log On to GitHub.  You should get a window like this.  Just enter you credentials to your GitHub account

![](/images/VScodeGITsetup_L.png)

12) At this point, you should be able to go to your GitHub page and view the project.

13)  If, for some reason, it does not work, you may have an old credential saved on your computer.  To correct this, you will need to delete the GitHub credential and re-login.  To do this, go to the Search box and type in "Credential Manager" and select it.

![](/images/VScodeGITsetup_J.png)

14) Click on "Windows Credentials" and look for  "GitHub " entry.  If it is there, you will want to "Remove" it so that you can re-login with your updated credentials

![](/images/VScodeGITsetup_K.png)

15) Try step 10) again and see if the Login window pops up.
