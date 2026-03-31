---
title: The Garden of Mirrors - VSeeFace on Linux
layout: page
filename: guide-vseeface-linux.md
--- 

# 3D Models / Model Tracking: VSeeFace

### ~Under construction, please wait warmly~

On Linux, a combination of the OpenSeeFace tracking tool and the VSeeFace animation tool is needed to 


First, if you don't already have them installed, install `git`, `python`, `python-pip` and `python-virtualenv` via command line. On Arch Linux, the command to do so is `pacman -S python python-pip python-virtualenv` (using `sudo` to run as administrator, or otherwise through root permissions).

Now, open a terminal in whatever folder you plan on installing your vtuber software to, or make one (e.g. with `mkdir` command).

Once you have the folder made, change to it (e.g. through `cd` command) and download the repository for the OpenSeeFace tracker through `git`:
```
git clone https://github.com/emilianavt/OpenSeeFace,
```

This copies the contents of the repository to your computer.

This installs the OpenSeeFace portion, but doesn't activate it yet. The next part will have to be run every time you start the face tracking system, and uses the OpenSeeFace piece to track your facial movements until you close the terminal window.

Switch to the OpenSeeFace folder that has been downloaded.

This next command sets up the virtual environment for the face tracker to run with:

```
virtualenv -p python3 venv && source venv/bin/activate && pip install onnxruntime opencv-python pillow numpy
```

What this does: "`virtualenv -p python3` " is the command to initialize a virtual python environment, specifically using Python 3. 

#### ~Under construction, please wait warmly~