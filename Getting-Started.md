# Getting started with the micro:bit

A quick guide to programming the micro:bit and saving your work on Github. This assumes you have done the following:
  - Installed [Python 3.7.2](https://www.python.org/downloads/) on your computer
  - Installed [PyCharm](https://www.jetbrains.com/pycharm/download/) on your computer
  - Installed [Git](https://git-scm.com/downloads) on your computer 
  - Installed [mu editor](https://codewith.mu/en/download) on your computer

## Github repository
1. Fork the [assignment repository](https://github.com/ivogeorg/micropython-tutorials.git)
2. Clone the forked repository to PyCharm.
3. Create a new file in the local repository clone, for example, `micropython-tut-01-hello-world.py`. Depending on your settings, the IDE will either ask you if you want to *git-add* the file to the repository, or will do it automatically. You can do an experimental *git-commit* to see if the file is added.
4. Copy over the code from the corresponding [MicroPython tutorial](https://microbit-micropython.readthedocs.io/en/latest/tutorials/hello.html). In this case it is:
   ```Python
   from microbit import *

   display.scroll("Hello, World!")
   ```

## The mu editor
1. Open the mu editor.
2. Click **Load**, find the file you just created, select it, and confirm. Now it appears in the mu editor. 

## The micro:bit
1. Connect the micro:bit device to your computer via the USB cable.
2. Wait for the new "drive" to appear on your desktop and/or in your file system.

## Flashing code
1. Back in the mu editor, click **Flash**.
2. Wait for the code to be converted to HEX and flashed to the ROM of the micro:bit device. The yellow reset LED on the back keeps flashing while this is being done, and stops when the process is complete. _**Note:** The micro:bit automatically resets the USB connection upon being flashed, which might result in your computer putting up an error message "Disk Not Ejected Properly". Don't worry about it. This is as it should be._
3. Your program starts executing right away, in this case scrolling *Hellow, World!* once.

## Wriring code
1. Modify the code in the mu editor. For example:
   ```Python
   from microbit import *

   display.scroll("Hello, MicroPython!")
   ```
2. Flash again and see it scroll.  
3. Repeat this process until you are satisfied with your program. 

## Saving your work
1. Since you opened the file from the local git repository, you will see the changes in PyCharm.
2. *git-commit* and *git-push* your changes to your remote.