# Button Clicker

This repository contains the project files for an electronic button clicker. A button clicker is a small electronic device that counts how many times the button on the device has been pressed. It features an additional button that displays the count on the device to save battery power. The maximum count on the device is 999,999, and it has a button debounce time of approximately 10ms. The counting mechanism utilizes BCD counters, and the count is displayed on 7-segment displays using a BCD to 7-segment IC. The device itself has dimensions of approximately 4 x 1 x 0.65 inches and comes with a 3D-printed case designed to hold the PCB. The PCB is a 2-layered board with a trace width and spacing of 0.15mm. Most components are surface mount devices (SMD), except for the buttons and displays. To ensure accurate functionality, it is recommended to add shielding inside the case; otherwise, the button clicker may randomly count up, reset, or count down. The electronics design was created using KiCad, while the case was made using FreeCAD. All design files are included in the repository, allowing for modifications if desired.

## Images

![Image 1](https://github.com/sam-was-here/button-clicker/assets/102840190/f6737c02-d3ff-409c-bf5a-29d78b7f556e)
![Image 2](https://github.com/sam-was-here/button-clicker/assets/102840190/d61c9d7f-647d-45af-8ad3-b09db66a89a1)
![Image 3](https://github.com/sam-was-here/button-clicker/assets/102840190/5f10ca7f-78ca-465b-a5b3-b0a1b61fc737)
![Image 4](https://github.com/sam-was-here/button-clicker/assets/102840190/2165c615-4cdc-498e-aa29-04d5a3c152f4)
![Image 5](https://github.com/sam-was-here/button-clicker/assets/102840190/05e833c8-f731-47f1-ad7b-6e20aca46a87)

## Bill of Materials (BOM)

- BT1: 3034TR - CR2032 battery holder - [Digi-Key Link](https://www.digikey.com/short/wqhf8fbf)
- C1-C11: 0603 0.1uF ceramic capacitor - bypass capacitor
- D1: SOD-523 - Crowbar diode for reverse polarity protection
- D2-D5: SMA - TVS diode - [Mouser Link](https://mou.sr/43r05RL)
- R1-R5: 0603 100k 5% resistor - button pull-up/down resistors and debouncing
- R6-R47: 0603 1k 5% resistor - LED current limiting resistors
- SW1: THT tack switch right angle - button for counting clicks - [Mouser Link](https://mou.sr/42t1Exi)
- SW2: THT tack switch right angle - button to light up display - [Mouser Link](https://mou.sr/42t1Exi)
- SW3: SMD tack switch - reset button - [Mouser Link](https://mou.sr/3oV6upt)
- U1: SOT-23 (5) 74LVC1G17 - Single Schmitt-Trigger Buffer - [Digi-Key Link](https://www.digikey.com/short/7bh4nv4q)
- U2-U4: TSSOP-16 74HC390 - Dual Decade RPL Counter - [Mouser Link](https://mou.sr/3katv4U)
- U5-U10: TSSOP-16 74HC4511 - BCD-to-7 Segment - [Digi-Key Link](https://www.digikey.com/short/bz3pz8r9)
- U11-U16: INND-TS30RCB - Red 7-segment display - [Digi-Key Link](https://www.digikey.com/short/40qw31cv)

## Schematic

![Schematic](button-clicker.pdf)

