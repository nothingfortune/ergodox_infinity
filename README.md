# ergodox_infinity

modified via application found here, export is only via json object

New firmware must be installed via Kiibohd Configurator

https://kiibohd.github.io/wiki/#/Quickstart

https://github.com/kiibohd/configurator/releases/download/v1.1.0/kiibohd-configurator-1.1.0-win.exe

Steps to Flash
1) Create Mapping inside of configurator
2) Take a backup JSON of your keymapping
3) Take a backup JSON of your keymapping!
4) Click "Flash keyboard"
    NOTE: Each half of this ergodox is considered it's "own" keyboard, so you will be flashing the same file twice, once for each half
5) Unplug the keyboards so only one is connected
6) On the bottom of the keyboard near the thumbcluster, there is a small hole with a button, this turns the keyboard into flash/bootloader mode
7) Click flash for the correct half of the keyboard
8) Repeat

NOTE: The configurator will crash if you enter bootloader mode and then click flash, so make sure that you have a backup json BEFORE you begin flashing.

Glossary
f1: momentary hold on a numbered layer, like &mo
latch-1: sends the user to the layer and button must be pressed again to send the user back to the original layer
next-f: sends the user to the next layer in sequence, based on numarical value of the layer itself (base 0 basis)
previous-f: sends the user to the next layer in sequence, based on numarical value of the layer itself
lock-1: locks the user to a particular layer, and this must be disabled before they can move to another layer