# The following walks you through the steps to install Git

1) [Download Git](https://git-scm.com/)

2) Run the install file and then walk through the default options with some key modifications:

![](/images/GitInstall_A.png)

3) In this next step, we are going to change where the software is installed to  `C:\Users\username\Git`

  You are going to click `Browse` and navigate to the `C:\Users` directory.  Then you are going to click on the subdirectriy that is your __`username`__. You should have the following in the text box (where you would just replace your __`username`__ in the entry).

  
  NOTE: Throughout the rest of the guide, you need to remember to replace __username__ with your username!


![](/images/GitInstall_B.png)

4) Make sure the following is checked.

![](/images/GitInstall_C.png)

5) Complete the installation making sure you select the options highlighted in red

![](/images/GitInstall_D.png)
![](/images/GitInstall_E.png)
![](/images/GitInstall_F.png)
![](/images/GitInstall_G.png)
![](/images/GitInstall_H.png)
![](/images/GitInstall_I.png)
![](/images/GitInstall_J.png)
![](/images/GitInstall_K.png)
![](/images/GitInstall_L.png)
![](/images/GitInstall_M.png)
![](/images/GitInstall_N.png)
![](/images/GitInstall_O.png)
![](/images/GitInstall_P.png)

6) Now that the software is installed, we need to complete a few steps to finish up.  Go to the Windows search box and type in "cmd"

![](/images/Command_A.png)

7) Then, click on the Command Prompt option above.  This will bring up command prompt window.

![](/images/Command_B.png)


`IMPORTANT: If the command window does not "pop-up", there may have been a previous uninstall issue.  Try the "Extra steps" below first!`


8) You may need to setup your username and email address for the Git software.  Type in the following at the prompt (where you replace "John Doe" with your name and "johndoe@example.com" with your email)
```
C:\Users\username>git config --global user.name “John Doe”
C:\Users\username>git config --global user.email johndoe@example.com
```

9) The following lists the configuration information.
```
C:\Users\username>git config --list
```
10) Just to be sure, let's make sure there are no __`.condarc`__ files in your __`C:\Users\username`__ directory.  Use the Windows File Explorer to delete them if they exist.

11) Next, you want to install [Miniforge](Miniforge.md)
---
<br>

## Extra Steps
### (ONLY when the command window won't start due to this error):

A) Make sure the __`auto run`__ part of the registry is cleared.  __`Please note that modifying the Registry can be harmful if you do not know what you are doing`__.  Go to the Windows search box and type this in

![](/images/RegEdit_A.png)

B) Click on the Registry Editor icon above

![](/images/RegEdit_B.png)

C) Navigate to the following section in the registry: __`Computer\HKEY_CURRENT_USER\SOFTWARE\Microsoft\CommandProcessor`__.  If you see an entry called __`AutoRun`__ that has the specfic following contents, you should right-click that entry and delete it.  

![](/images/RegEdit_C.png)

D) When you are done, it should be removed (like below)

![](/images/RegEdit_D.png)

E) At this point, you should be able to go back to step 6) and complete this part of the install.
