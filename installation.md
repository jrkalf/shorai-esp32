# Prerequisites

## Install Micropython on your ESP32
You should have an ESP32 device installed with Micropython.
You can find the micropython firmware and installation instructions here: https://micropython.org/download/

## Install Thonny or uPyCraft IDE

Thonny: https://thonny.org
uPyCraft: https://github.com/DFRobot/uPyCraft

## prepare the shorai-esp32 config

Download the latest version of Toremick's github repository and modify the config.py file to fit your configuration.


# Installation

1. Open Thonny
2. Make sure the right interpreter is selected
3. Make sure the right Port or WebREPL is selected
4. Open files (config.py, main.py and all files in the main/ subfolder)
5. press "save as" for each file and select you want to write them to the micropython.
6. Be sure to put config.py and main.py next to the boot.py
7. Be sure to create a subfolder called main to install all other files in there.
8. When you're in a "Save As" window, rightclick the boot.py and delete this file. You'll no longer need this.

Alternatively you can run this command on the thonny terminal:

```python
import os
os.listdir()
os.remove("/boot.py")
os.listdir()
```

The code above does a list dir to show you the boot.py is still there, then removes it, then does another list dir to confirm it's gone.
Then press CTRL-D to soft reset the board and start running the code.