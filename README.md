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
1. Hold the BOOTSEL switch while plugging the board into the computer (or map the key onto another keyboard). Your computer will recognize the keyboard as a new USB flash drive.
2. Drag the .uf2 firmware file onto the drive which will flash and reconnect as your keyboard.

## BOM for everything but the PCB
These are just items I found online, obviously not everyone will have to buy everything or may find things cheaper.
| Item | Price | 
| -------- | -------- | 
| PORON Foam 3mm (https://kineticlabs.com/misc/kinetic/keyboard-case-foam) | $11.99 | 
| PORON Switch Pads 120pcs (https://www.thockking.com/products/120-pcs-poron-switch-pcb-pads-keyboard?srsltid=AfmBOoo6HK_r0ljKCA8shWPgEShMNSKvCRTplPMlUFCUZeMBYEVjpXQe) | $5.95 |
| PORON Gasket Pack (https://sneakbox.com/products/poron-gasket-pack-for-ava) | $2.50 |
| Rubber Feet for Grip 16pcs (https://www.amazon.com/Non-Slip-Replacement-Compatible-Keyboard-Appliance/dp/B0D4YMSKB4/ref=sr_1_11?dib=eyJ2IjoiMSJ9.XoUMk7-UOlTtPtFYWQZpOQQ0YV07qMV2vTZ3kSxIkSIlizGofOPVbTpGYzwRQw88zKSM_KaKzUI6qV4OeunmTbTU3q4nR0jaM8CfstdL5DCAXgpC3ANQ_niT6N3AHx2a1g9P4uldjTluwpxN1PMmYOOq9HpF6IvnZPEHAniQHR3mgzZNr9sqDr-lmo_pEqo7xObI15IINl3HmPJ3EgNBM4ETJDI--IO8IAdWWZ-Z_FE.Q2DZ8wJYTM9evpEy83jlTd3WV4KQYcCodQErPj6XfDI&dib_tag=se&keywords=computer+bottom+grips&qid=1783888312&sr=8-11) | $5.99 |
| PLA Jade White Filament - Refills (https://us.store.bambulab.com/products/pla-basic-filament?id=40475106640008&skr=yes&srsltid=AfmBOopkMxBwVVOAUPB-eUb1OnMVHz0YslsCtdrWvmvNn3WDPF1wTifkfaI) | $19.99 |
| PLA Dark Gray Filament - Refills (https://us.store.bambulab.com/products/pla-basic-filament?id=42844629008520&skr=yes&srsltid=AfmBOopkMxBwVVOAUPB-eUb1OnMVHz0YslsCtdrWvmvNn3WDPF1wTifkfaI) | $19.99 |
| Kailh Box White Mechanical Switches 108pcs (https://www.amazon.com/Zjmehty-Mechanical-Keyboard-Switches-Waterproof/dp/B0CBPQGBSF/ref=sr_1_3?dib=eyJ2IjoiMSJ9.E0cY7EpgxNWIGrjiUDijL2yX7QuJ4sSXQ3ni0V0YHDAgaGYgADZFwBu84mjhf-QysIyrwlpTxvjmzL0KDfYxlYY83vHiW4xgVClPXeF4Ib92ppCQysXUy_H-mAxLtrBvZS-ZL3z2GxEdb6f2pQ4qCblsv-kbjjwNlKHZ9bSdp37dGywsIBQwMoVVzmxqHsSfLnByHLKTMRRTwjsypfUzWYkZ373k-XDaxMY0TNUJ_mk.5vlHIp12Un8F6nijEipLgdprO-QfBAuDYCqbvLERydk&dib_tag=se&keywords=kailh%2Bswitches&qid=1783899117&sr=8-3&th=1) | $32.99 |
| Black on White Double Shot ABS Keycap Set 150pcs (https://mechanicalkeyboards.com/products/tai-hao-150-key-abs-double-shot-cubic-keycap-set-black-on-white) | $23.99 |
| M3x25mm + M3x35mm Screws (https://www.amazon.com/VGBUY-443Pcs-Assortment-Printer-Washers/dp/B0D14BC8QS/ref=sr_1_29?dib=eyJ2IjoiMSJ9.cJlzu8DHjxsBzA9lFsc42RrAUiLpBy2F3tkct2TerB3jPoWxLy1FFqgPkZL65Hm6hQ30CzHtc9XbV1b-KKiqKPhDFOW3YmMjd30Ejia8Nu6dS_fYUZJw2OaXmPkm66xulz6iDtLy41kDzPSHcQoN8hYNtvkRf0d3jzQRr0kr6lgkEKZoX19UdRjpKiqxOx5Y.NBmS5v4xF-mHcY9zdglMfK5eDmRY_j0mqYXsMdjWDFA&dib_tag=se&keywords=metric%2Bscrews%2Bm3&qid=1783871590&sr=8-29&xpid=46NRh2P79qy-c&th=1) | $9.99 |
| Stabilizers (https://minokeys.com/products/aeboards-staebies) | $20.00 | 
| Total: | $147.39 | 

## Assembly (a little unconventional but I plan on making things easier in the future)
1. Case Dampening - Cut the 3mm PORON case FOAM to fit and lay it fly inside the 3D-printed bottom case. There should be a 1.5 mm air gap between the foat and the hotswap sockets to allow for gasket flex. Extra foam can be placed but they shouldn't be overpacked.
2. PCB + Plate - Apply the PORON switch pads to the the PCB, install the stabilizers, and snap your chosen switches into the plate to secure them. Align the switch pins with the Kailh hotswap sockets and press the plate and PCB together.
3. Gasket Mounting - Apply the PORON Gaskets to all four margins on the plate, one on the top of the plate and the other on the bottom, creating a sandwich. These gaskets should rest on the shelf located in the bottom case.
4. Case Fastening - Place the top case over the assembly and secure it by driving screws through the matching holes on the bottom case. This current case design calls for M3 x 23mm screws on the front end of the keyboard and M3 x 34mm screws on the back end, which are not standard screw sizes and are hard to source. Trim M3 x 25mmm and M3 x 35mm screws accordingly if the custom sizes cannot be found. Future changes to the design will utilize standard screw sizes.
5. Keycaps - Add your desired keycaps according to the chosen layout and plug in the keyboard.

