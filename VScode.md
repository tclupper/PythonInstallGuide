# The following walks you through the steps used to install Visual Studio Code
(This is the default development IDE that I use.  You can use a different one)

1) [Download VScode](https://code.visualstudio.com/)

2) Install VScode with all the default options

3) We have to make sure VScode can access the Python scripts located in __`C:\Users\username\Miniforge3\Scripts`__.  To do this, go to the Windows search box and type in "environment".  You should see the icon above to edit the environment variables

![](/images/EnvironmentVariables_A.png)

4) After you click on this, it will bring up the __`System Properties`__ window.  Click on the __`Environment Variables`__ button.

![](/images/EnvironmentVariables_B.png)

5) Next, select the __`Path`__ variable in the __`User Variables`__ section.  Then, and click on __`Edit`__

![](/images/EnvironmentVariables_C.png)

6) Next, click on the __`New`__ button and add the following path to the list.  Remember to replace your __`username`__ in the path.
```
C:\Users\username\miniforge3\Scripts
```

7) Install the Extensions you wish.  I installed the following:
    - Anaconda Extension Pack
    - Code Spell Checker
    - Dracula Official
    - GItLens - Git Supercharged
    - Jupyter
    - Live Sass Compiler
    - Live Server
    - Pylance
    - Python
    - SQL Server (mssql)
    - Visual Studio Intellicode
    - vscode-pdf
    - YAML

