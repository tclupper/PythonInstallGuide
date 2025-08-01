# The following walks you through the steps to install Miniforge
 * This is a trimmed down version of [Anaconda](https://anaconda.org/) without the user interface.  I used [Miniconda](https://docs.conda.io/en/latest/miniconda.html) at first, but found that the packages in the repository were older.  Minforge uses the [Conda-Forge](https://conda-forge.org/) repository.

1) [Download Miniforge](https://conda-forge.org/download/)

![](/images/MiniforgeInstall_A.png)

2) Run the install file and then walk through the default options with key modifications:

`NOTE:  you may get this exception when you try and run it (I did).  I just clicked the "Run anyway" option to continue.`

![](/images/MiniforgeInstall_B.png)
![](/images/MiniforgeInstall_C.png)

Start the process:

![](/images/MiniforgeInstall_D.png)
![](/images/MiniforgeInstall_E.png)
![](/images/MiniforgeInstall_F.png)

3) In this next step, we are going to change where the software is installed to  `C:\Users\username\Miniforge3`

  You are going to click `Browse` and navigate to the `C:\Users` directory.  Then you are going to click on the subdirectriy that is your __`username`__. You should have the following in the text box (where you would just replace your __`username`__ in the entry)

![](/images/MiniforgeInstall_G.png)
![](/images/MiniforgeInstall_H.png)
![](/images/MiniforgeInstall_I.png)
![](/images/MiniforgeInstall_J.png)

4) Now that the software is installed, we need to create a basic Python environment that can run Jupyter Lab and write Python programs.  To do this, you need to open a command prompt where the **base** miniforge environment is enabled.  Go to the Windows Programs menu, find and click on the `Miniforge Prompt` option.

![](/images/MiniforgeInstall_K.png)

5) You will get a command window that has the following prompt:

```
(base) C:\Users\username>
```
`IMPORTANT: If a command window does not "pop-up", there may have been a previous uninstall issue.  Try the "Extra steps" at the end of the Git install section first!`

You will need to update the Conda environment. To do this, type this:
```
C:\Users\username>conda update --all
```

6) Next, type in the following to create a basic Python environment that I am going to call "py".  You can use a different name than "py" if you wish.  (Type "Y" to complete the process)
```
(base) C:\Users\username>conda create -n py python=3
```

7) I have created a list of packages that I feel are necessary for most engineering type problems in Python and [Jupyter Lab](https://jupyter.org/).  You can modify this is needed.  You are going to want to download this [requirements.txt](https://raw.githubusercontent.com/tclupper/PythonInstallGuide/master/requirements.txt) file into your *Documents* directory.  Just "Right-Click" on the page as select "Save-As..." to download file.

8) Next, open up the (base) window as shown in step 4) and type the following (Replacing "username" with your username)
```
(base) C:\Users\username>activate py
(py) C:\Users\username>cd C:\Users\username\Documents
(py) C:\Users\username\Documents>conda install --file requirements.txt
```
At this point, you have a basic Python enviroment that you can use to write programs and run Jupyter Lab.

---
## Additional (but important) Steps
* Enable both the Windows command prompt and the Windows Power Shell prompt to start with "conda" environments available
  * This is really optional (a matter of preference)
* Add Windows Start menu shortcuts for the applications
  * I find this extremely helpful
* Enable Jupyter Lab to start as a stand-alone application
  * If you want to open a document from any folder on your c:\ drive
---

9) First, open a new command window as shown in step 4) & 5) and type in the following command
```
(base) C:\Users\username>conda init --reverse cmd.exe powershell
```
10) Next, close that window and then open a __Power Shell__ window by typing power shell in the search bar

![](/images/CondaInit_A.png)
![](/images/CondaInit_B.png)

11) Type in the following commands.  Make sure to type "Y" when needed.  When, finished, close that window.
```
PS C:\Users\username>Set-ExecutionPolicy -Scope CurrentUser RemoteSigned
```
12) Now, open back up a command window as shown in step 4) & 5) and type the following.
```
(base) C:\Users\username>conda init cmd.exe powershell
```

13) We have to make sure the system can access conda and Python located in __`C:\Users\username\miniforge3\condabin`__.  To do this, go to the Windows search box and type in "environment".  You should see the icon above to edit the environment variables

![](/images/EnvironmentVariables_A.png)

14) After you click on this, it will bring up the __`System Properties`__ window.  Click on the __`Environment Variables`__ button.

![](/images/EnvironmentVariables_B.png)

15) Next, select the __`Path`__ variable in the __`User Variables`__ section.  Then, and click on __`Edit`__

![](/images/EnvironmentVariables_C.png)

16) Next, click on the __`New`__ button and add the following path to the list.  Remember to replace your __`username`__ in the path.
```
C:\Users\username\miniforge3\condabin
```

Now, when you open a Power Shell window, it will come up with (base) environment enabled by default.  Also, when you open a standard CMD window, all you have to do is type `activate` to activate the (base) environment.

---
17) Next, we will create the Windows Start menu shortcuts. Download the files in the [__`Menu`__](https://github.com/tclupper/PythonInstallGuide/tree/master/menu) directory of this repository and put them in the following directory on your computer:
__`C:\Users\username\miniforge3\Menu`__.  To do this, open the [__`Menu`__](https://github.com/tclupper/PythonInstallGuide/tree/master/menu) directory and then click on each file separately and select the view "Raw" option.  Then "Right-Click" and select "Save-as..." or "Save image as..." for each of the files, depending on the file type.

![](/images/MenuDirectory_A.png)

18) Next, open up another (base) command window as described in step 4) & 5) and type the following
```
(base) C:\Users\username>cd C:\
(base) C:\>menuinst C:\Users\username\miniforge3\Menu\baseCMDconsole_shortcut.json
(base) C:\>menuinst C:\Users\username\miniforge3\Menu\basePSconsole_shortcut.json
(base) C:\>menuinst C:\Users\username\miniforge3\Menu\pyCMDconsole_shortcut.json
(base) C:\>menuinst C:\Users\username\miniforge3\Menu\pyPSconsole_shortcut.json
(base) C:\>menuinst C:\Users\username\miniforge3\Menu\Jupyterlab_shortcut.json
```

This should install/place shortcuts in the Start menu so you can directly open windows with conda environments activated or run JupyterLab directly.  Go look at the Windows Start menu under __`Miniforge3`__.  You should see the following:

![](/images/MenuDirectory_B.png)

---

The final setp is to make sure Jupyter Lab opens in a [" Desktop application-like"](http://christopherroach.com/articles/jupyterlab-desktop-app/) environment, as well as allowing you to open notebooks from directories that start at the root, or C:\\.

19) Using the new menus that we just created, open an `Miniforge CMD Prompt (py)` window and Type the following commands.

```
(py) C:\Users\username\Documents>jupyter lab --generate-config
```

This will create the following directory and file (which you will want to edit using a text editor like Notepad++)

`C:\Users\username\.jupyter\jupyter_lab_config.py`

Now, when you edit the file, there will be a lot of stuff in it. Find where you see the following within the file:
```
## Specify what command to use to invoke a web
# browser when starting the server. If not specified, the
# default browser will be determined by the `webbrowser`
# standard library module, which allows setting of the
# BROWSER environment variable to override it.
#  Default: ''
# c.ServerApp.browser = ''
```
If you have `Google Chrome` installed, you would modify the last line to look like this (*__don't forget to remove the hash at the begining__*):
* c.ServerApp.browser = 'C:/Program Files (x86)/Google/Chrome/Application/chrome.exe --app=%s'

or, if Chrome is installed in /Program Files/ , then use this
* c.ServerApp.browser = 'C:/Program Files/Google/Chrome/Application/chrome.exe --app=%s'

However, if you are going to use `Microsoft Edge`, you would modify the last line to look like this (*__don't forget to remove the hash at the begining__*):
* c.ServerApp.browser = 'C:/Program Files (x86)/Microsoft/Edge/Application/msedge.exe --app=%s'

or, if Edge is installed in /Program Files/ , then use this
* c.ServerApp.browser = 'C:/Program Files/Microsoft/Edge/Application/msedge.exe --app=%s'


Or, if you are going to use `Mozilla Firefox`, you would modify the last line to look like this (*__don't forget to remove the hash at the begining__*):
* c.ServerApp.browser = 'C:/Program Files (x86)/Mozilla Firefox/firefox.exe --app=%s'


Next, where you see this:
```
## The directory to use for notebooks and kernels.
#  Default: ''
# c.ServerApp.root_dir = ''
```
Modify this line (In order to start Jupyter Lab at C:\\). (*__Also, don't forget to remove the hash at the begining__*)
* c.ServerApp.root_dir = 'C:\\\\'
---

20) Next, you want to install [VScode](VScode.md)

---
---

## These last steps are optional, or just for your info.

If you want to list general information about an environment, type this:
```
(py) C:\Users\username>conda info
```

If you want to update any enviroment, type this:
```
(py) C:\Users\username>mamba update --all
```

If you want to list what packages are in an enviroment, type this:
```
(py) C:\Users\username>conda list
```

If you are in the "base" enviroment and want to activate the "py" enviroment, then type this: 
```
(base) C:\Users\username>conda activate py
```

If you want to create a new enviroment (say called, "pyprog") with just a few packages, not the whole anaconda list, then type this:
```
(base) C:\Users\username>conda create -n pyprog python numpy matplotlib pyinstaller
(base) C:\Users\username>conda activate pyprog
(pyprog) C:\Users\username>
```

To list the availble environments, type this:
```
(base) C:\Users\username>conda env list
```

To delete an environment, type this:
```
(base) C:\Users\username>conda env remove -n pyprog
```
Then, remember to delete the folder:
* C:\Users\username\miniconda\envs\pyprog
