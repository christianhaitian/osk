Originally from the Retropie Project: https://github.com/RetroPie/RetroPie-Setup/blob/master/scriptmodules/admin/joy2key/osk.py
<p align="left"><img width="640" height="382" src="https://github.com/christianhaitian/osk/raw/main/osk_screenshot.JPG"></p>

## To install and use this

Requirements: \
Python 3.5 or newer \
Python3 urwid module

In ArkOS, Python 3.7 is already included.  To install the urwid module, do `sudo apt -y update && sudo apt -y -t eoan install python3-urwid`

To run this from within a ssh terminal, just make sure osk.py is executable `chmod 755 osk.py`, then execute it.  You can also call it with python3 (ex. python3 osk.py)

To run this so it outputs on a builtin screen, you need to add `2>&1 > /dev/tty1` to the end of the execution line for it. (ex. osk.py 2>&1 > /dev/tty1)

To use this directly on your device, you will need a keyboard emulator such as [gptokeyb](https://github.com/christianhaitian/gptokeyb) or [oga_controls](https://github.com/christianhaitian/oga_controls).  gptokeyb is recommended as it is more up-to-date.

commandline switch options: \
--backtitle "Backtitle" (Change the background title to some other text.  Default is ArkOS) \
--inputbox "inputbox" (Add a title to the input box itself.  This switch is not needed as it's assumed the text added after the osk.py executable is the title of the inputbox) \
--minchars "number" (Require the user to enter a minimum number of characters before accepting the input)
