# Installation instructions for a Python environment on a Microsoft Windows-based computer

## Rev 5/27/2024
<br>

### NOTE: The official URL for this guide is:  https://github.com/tclupper/PythonInstallGuide 
<br>

This is a step-by-step guide to install software on your computer for the development of Python programs and Jupyter notebooks.  I put this guide together mostly to document the process that I use.  Your mileage may vary.

You will need the following 4 software titles. I recommend installing them in the following order:

1) [Notepad++ (ver 8.6.7)](NotepadPlusPlus.md) (This is the text editor that I use)
2) [Git (ver 2.45.1](Git.md)  (This is used for version control of text based files, i.e. source code, jupyter notebooks, static files, etc.)
3) [Miniforge3 (ver 24.3.0-0)](Miniforge.md)  (Stripped down version of Anaconda)
4) [VScode (ver 1.89.1)](VScode.md)  (This is the development IDE that I use)
---
## Just as an FYI, Here is a list of other free software that I use
* For Visual Basic and C# applications, I use [Visual Studio Community 2022 (ver 17.10.0)](https://visualstudio.microsoft.com/vs/community)

* Office suite
    * [Libre Office (ver 24.2.3)](https://www.libreoffice.org)
* Latex document editor
    * [Texworks/MikTex (ver 0.6.8/ver 24.1)](https://miktex.org/download)
* Sound recorder/editor
    * [Audacity (ver 3.5.1)](https://www.audacityteam.org)
* Image viewing, creating and editing
    * [IRfanView (ver 4.67)](https://www.irfanview.com)
    * [Paint.net (ver 5.0.13)](https://www.getpaint.net)
    * [ImageJ (ver 1.54i)](https://imagej.nih.gov/ij/)
* Vector graphics viewing, creating and editing
    * [Inkscape (ver 1.3.2)](https://inkscape.org)
    * [DrawIO Desktop (ver 24.4.8)](https://github.com/jgraph/drawio-desktop/releases)
* 2D mechanical drawing
    * [LibreCAD (ver 2.2.0.2)](https://github.com/LibreCAD/LibreCAD/releases)  (Not sure about this one, I may just switch to FreeCad for everything)
* 3D mechanical drawing and modeling
    * [OpenSCAD (ver 2021.01)](https://openscad.org/downloads.html)
    * [FreeCAD (ver 0.21.2)](https://www.freecadweb.org)
* 3D printing utilities
    * [PrusaSlicer (ver 2.7.4)](https://www.prusa3d.com/prusaslicer)
    * [Cura (ver 5.7.1)](https://ultimaker.com/software/ultimaker-cura)
    * [MeshLab (ver 2023.12)](https://www.meshlab.net/#download)
* EE specific tools
    * [KiCAD (ver 8.0.2)](https://kicad.org/download/windows/) ~Schematic capture and PCB layout
    * [LTspice (ver 24.0.12)](https://www.analog.com/en/design-center/design-tools-and-calculators/ltspice-simulator.html) ~Circuit simulation
    * [Arduino IDE (ver 2.3.2)](https://www.arduino.cc/en/software) ~IDE for Arduino control boards
    * [Putty (ver 0.81)](https://www.putty.org) ~Communication tool
    * [EZNEC Pro/2+ (ver 7.0.2)](https://www.eznec.com/) ~Wire antenna simulation. Final version.
    * [Chirp-next (ver 20240514)](https://chirp.danplanet.com/projects/chirp/wiki/Download) ~HAM radio programming software
    * [AADE filter design (ver 4.5)](http://www.ke5fx.com/aadeflt.htm) ~Lumped element filter design. Final version.
    * [METAS VNA tools (ver 2.8.2)](https://www.metas.ch/metas/en/home/fabe/hochfrequenz/vna-tools.html)~Nice set of S-parameter display and calibration uncertainty tools if you use a vector network analyzer
* Utilities
    * [Free 42 (ver 3.1.8)](https://thomasokken.com/free42/) ~HP42S calculator app
    * [Convert (ver 4.1.0e)](https://joshmadison.com/convert-for-windows/) ~Unit conversion app
    * [7-Zip (Ver 24.06)](https://www.7-zip.org/) ~File Compression