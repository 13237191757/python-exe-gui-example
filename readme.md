#Python GUI Executable App Example

This example evaluates the various packages that can be used to 
generate a standalone python executable App in windows.
Similar to the [Command line App example](https://github.com/boseji/python-exe-commandline-example) this 
is the GUI version. It uses TCL/TK to create a basic main window demonstarting a simple GUI app.

## Python Version

This example was tested in [`python 2.7.9`](https://www.python.org/downloads/release/python-279/) 
on an **Windows 7 64-bit based PC**.

Assuming that the Python instllation happend in he directory `C:\Python27` and 
there is a *Script Directory* at `C:\Python27\Scripts`.

## Executable conveter Packages Tested

1. [Py2Exe](http://www.py2exe.org/)
2. [cx-Freeze](http://cx-freeze.sourceforge.net/)
3. [PyInstaller](https://github.com/pyinstaller/pyinstaller/wiki)

All the above three need to configured to be able to installed to execute the individual examples.

## Environment Initialization

1. Open Command prompt using `cmd` command in *Start Menu*
2. Enter Command `SET PATH=C:\Python27;C:\Python27\Scripts;%PATH%` to 
    make sure that the `Scripts` directory is in **PATH** environment variable
    This ensures that the Path is configured properly and have access to python package manager.
3. Now for `pip` installations use the following Commands:

    `pip install cx_freeze PyInstaller virtualenv`
    
    `pip install wget` - In case one needs a download manager
    
    `pip install --upgrade cx_freeze PyInstaller virtualenv` - For upgradation

4. Download the Py2exe Installations:
    -  Installer For [64bit](http://goo.gl/teSXF8) and [32bit](http://goo.gl/Q3G5q) are available.
    -  Install any one of them depending upon the type of system Architecture. In our case it was a 64-bit one.
    -  The Package Files are located at: http://sourceforge.net/projects/py2exe/files/py2exe/ 
       In case there are any new releases of the Py2exe package
    -  We are using the [0.6.9 version of Py2exe](http://sourceforge.net/projects/py2exe/files/py2exe/0.6.9/)

5. Download the PyWin32 Installation:
    -  Installers For [64bit](http://goo.gl/Ew5uEx) and [32bit](http://goo.gl/RS7SJQ) are avaiable
    -  Install any one of them depending upon the type of system Architecture. In our case it was a 64-bit one.
    -  The Package Files are located at: 
        http://sourceforge.net/projects/pywin32/files/pywin32/ 
        In case there are any new releases of the PyWin32 package
    -  We are using the 
    [Build 219 Version of PyWin32](http://sourceforge.net/projects/pywin32/files/pywin32/Build%20219/)

With these we are ready to for creation of the executable Apps.


