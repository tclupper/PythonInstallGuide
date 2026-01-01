# Installation instructions for a Python environment on a Microsoft Windows-based computer

## Rev 1/1/2026 
<br>

### NOTE: The official URL for this guide is:  https://github.com/tclupper/PythonInstallGuide 
<br>

This is a step-by-step guide to install software on your computer for the development of Python programs and Jupyter notebooks.  I put this guide together mostly to document the process that I use.  Your mileage may vary.

You will need the following 4 software titles. I recommend installing them in the following order:

1) [Notepad++ (ver 8.9.0)](NotepadPlusPlus.md) (This is the text editor that I use)
2) [Git (ver 2.52.0)](Git.md)  (This is used for version control of text based files, i.e. source code, jupyter notebooks, static files, etc.)
3) [Miniforge3 (ver 25.11.0-1)](Miniforge.md)  (Stripped down version of Anaconda)
4) [VScode (ver 1.107.1)](VScode.md)  (This is the development IDE that I use)

NOTE: Jupyter notebooks are best edited using JupyterLab (installed via the Miniforge distribution).  However, with the proper extensions installed, you can use VScode to edit Jupyter notebooks, Latex documents, CSS/HTML/Flask apps, as well as Python programs that use tkinter UI.

## Just as an FYI, Here is a list of other free software that I recommend
* For Visual Basic and C# applications, I use [Visual Studio Community 2022 (ver 17.14.23)](https://visualstudio.microsoft.com/vs/community)

* Office suite

    * [Libre Office (ver 25.8.4)](https://www.libreoffice.org)
* Latex document editor
    * [Texworks/MikTex (ver 0.6.10/ver 25.12)](https://miktex.org/download)
* Reference material manager
    * [Zotero (ver 7.0.30)](https://www.zotero.org/download/)
* Sound recorder/editor
    * [Audacity (ver 3.7.7)](https://www.audacityteam.org)
* Image viewing, creating and editing
    * [IRfanView (ver 4.7.3)](https://www.irfanview.com)
    * [Paint.net (ver 5.1.11)](https://www.getpaint.net)
    * [ImageJ (ver 1.54r)](https://imagej.net/)
    * [DigiCamControl (ver 2.1.7)](https://www.digicamcontrol.com/download)
* Vector graphics viewing, creating and editing
    * [Inkscape (ver 1.4.3)](https://inkscape.org)
    * [DrawIO Desktop (ver 29.0.3)](https://github.com/jgraph/drawio-desktop/releases)
* 2D mechanical drawing
    * [LibreCAD (ver 2.2.1.2)](https://github.com/LibreCAD/LibreCAD/releases)
* 3D mechanical drawing and modeling
    * [OpenSCAD (ver 2025.12.30)](https://openscad.org/downloads.html)
    * [FreeCAD (ver 1.0.2)](https://www.freecadweb.org)
* 3D printing utilities
    * [PrusaSlicer (ver 2.9.4)](https://www.prusa3d.com/prusaslicer)
    * [MeshLab (ver 2025.07)](https://www.meshlab.net/#download)
* EE specific tools
    * [KiCAD (ver 9.0.6)](https://kicad.org/download/windows/) ~Schematic capture and PCB layout
    * [LTspice (ver 26.0.1)](https://www.analog.com/en/design-center/design-tools-and-calculators/ltspice-simulator.html) ~Circuit simulation
    * [Arduino IDE (ver 2.3.7)](https://www.arduino.cc/en/software) ~IDE for Arduino control boards
    * [Putty (ver 0.83)](https://putty.software/) ~Communication tool
    * [EZNEC Pro/2+ (ver 7.0.4)](https://www.eznec.com/) ~Wire antenna simulation. Final version.
    * [Chirp-next (ver 20251219)](https://chirp.danplanet.com/projects/chirp/wiki/Download) ~HAM radio programming software
    * [AADE filter design (ver 4.5)](http://www.ke5fx.com/aadeflt.htm) ~Lumped element filter design. Final version.
    * [METAS VNA tools (ver 2.9.4)](https://www.metas.ch/metas/en/home/fabe/hochfrequenz/vna-tools.html)~Nice set of S-parameter display and calibration uncertainty tools if you use a vector network analyzer
* Utilities
    * [Free 42 (ver 3.3.10)](https://thomasokken.com/free42/) ~HP42S calculator app
    * [Convert (ver 4.1.0e)](https://joshmadison.com/convert-for-windows/) ~Unit conversion app
    * [7-Zip (Ver 25.01)](https://www.7-zip.org/) ~File Compression
    * [ShareX (Ver 18.01)](https://getsharex.com/) ~Screen capture