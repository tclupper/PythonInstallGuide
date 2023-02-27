# Installation instructions for a Python environment on a Microsoft Windows-based computer
## Rev 2/27/2023
<br>

### NOTE: The official URL for this guide is:  https://github.com/tclupper/PythonInstallGuide 
<br>

This is a step-by-step guide to install software on your computer for the development of Python programs and Jupyter notebooks.  I put this guide together mostly to document the process that I use.  Your mileage may vary.

You will need the following 4 software titles. I recommend installing them in the following order:

1) [Notepad++ (ver 8.4.9)](NotepadPlusPlus.md) (This is the text editor that I use)
2) [Git (ver 2.39.2](Git.md)  (This is used for version control of text based files, i.e. source code, jupyter notebooks, static files, etc.)
3) [Miniforge3 (ver 22.11.1-4)](Miniforge.md)  (Stripped down version of Anaconda)
4) [VScode (ver 1.75.1)](VScode.md)  (This is the development IDE that I use)
---
## Just as an FYI, Here is a list of other free software that I use
* For Visual Basic and C# applications, I use [Visual Studio Community 2022 (ver 17.5.0)](https://visualstudio.microsoft.com/vs/community)

* Office suite
    * [Libre Office (ver 7.5.0.3)](https://www.libreoffice.org)
* Sound recorder/editor
    * [Audacity (ver 3.2.4)](https://www.audacityteam.org)
* Image viewing, creating and editing
    * [IRfanView (ver 4.62)](https://www.irfanview.com)
    * [Paint.net (ver 5.02)](https://www.getpaint.net)
    * [ImageJ (ver 1.54b)](https://imagej.nih.gov/ij/)
* Vector graphics viewing, creating and editing
    * [Inkscape (ver 1.2.2)](https://inkscape.org)
    * [DrawIO Desktop (ver 20.8.16)](https://github.com/jgraph/drawio-desktop/releases)
* 2D mechanical drawing
    * [LibreCAD (ver 2.2.0)](https://github.com/LibreCAD/LibreCAD/releases)
* 3D mechanical drawing and modeling
    * [OpenSCAD (ver 2021.01)](https://openscad.org/downloads.html)
    * [FreeCAD (ver 0.20.2)](https://www.freecadweb.org)
* 3D printing utilities
    * [PrusaSlicer (ver 2.5.0)](https://www.prusa3d.com/prusaslicer)
    * [Cura (ver 5.2.2)](https://ultimaker.com/software/ultimaker-cura)
    * [MeshLab (ver 2022.02)](https://www.meshlab.net/#download)
* EE specific tools
    * [KiCAD (ver 7.0.0)](https://kicad.org/download/windows/) ~Schematic capture and PCB layout
    * [LTspice (ver 17.1.6)](https://www.analog.com/en/design-center/design-tools-and-calculators/ltspice-simulator.html) ~Circuit simulation
    * [Arduino IDE (ver 2.0.4)](https://www.arduino.cc/en/software) ~IDE for Arduino control boards
    * [Putty (ver 0.78)](https://www.putty.org) ~Communication tool
    * [EZNEC Pro/2+ (ver 7.0.1)](https://www.eznec.com/) ~Wire antenna simulation. Final version.
    * [Chirp-next (ver 20230224)](https://chirp.danplanet.com/projects/chirp/wiki/Download) ~HAM radio programming software
    * [AADE filter design (ver 4.5)](http://www.ke5fx.com/aadeflt.htm) ~Lumped element filter design. Final version.
    * [METAS VNA tools (ver 2.6.2)](https://www.metas.ch/metas/en/home/fabe/hochfrequenz/vna-tools.html)~Nice set of S-parameter display and calibration uncertainty tools if you use a vector network analyzer
* Utilities
    * [Free 42 (ver 3.0.17)](https://thomasokken.com/free42/) ~HP42S calculator app
    * [Convert (ver 4.1.0)](https://joshmadison.com/convert-for-windows/) ~Unit conversion app
    * [7-Zip (Ver 22.01)](https://www.7-zip.org/) ~File Compression