# TKL Keyboard
An F12 TKL Multi-Layout Hotswap keyboard, designed in KiCad10 and Fusion360. Everything in the 'Production' folder of this repository should be everything you need for the physical parts of this keyboard. Gerbers file can be provided to JLCPCB (or others) for them to manufacture the PCB. The STP files are used to 3D print the top case, bottom case, and plate.

KiCad Renders:
### ![PCB Front](Assets/3dpcbfront.png)
### ![PCB Back](Assets/3dpcbback.png)

Keyboard Case:
### ![Entire Case](Assets/finishedkeyboard.png)
### ![Exploded Case](Assets/explodedkeyboardcase.png)

## Features
* RESET Switch - allows you to reboot the keyboard's processor 
* BOOTSEL Switch - Allows you to load custom firmware onto the keyboard
* Uses the RP2040 MCU
* Uses Kailh Hotswap Sockets
* 16Mib Flash Memory
* 12MHz Crystal
* USB-C Port
* ESD Chip to prevent damage from electrostatic discharge
* Supports ANSI/ISO

## Multi-Layout Support
### ![Multi-Layout](Assets/keyboard-layout.png)

## Firmware
Here's the basic keyboard layout (the one included in the 'Firmware' folder):
### ![Keyboard Layout](Assets/keymapping.png)
You can edit it by uploading the JSON file in the 'Firmware' folder into QMK and making the necessary changes for the layout you want to use.
### Flashing Instructions
Hold the BOOTSEL switch while plugging the board into the computer (or map the key onto another keyboard). Your computer will recognize the keyboard as a new USB flash drive. Then, drag the .uf2 firmware file onto the drive which will flash and reconnect as your keyboard.
