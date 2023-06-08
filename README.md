# button-clicker
This is the repo for a electronic button clicker. A button clicker is a small electronic device that counts how many times the button on the devices was pressed. there is another button that show the count on the device to save battery. The max count on the deive is 999,999 and has a button debounce time of about 10ms. all the counting is done with BCD counters and is displayed on 7 segment displays usesing BCD to 7 segment IC. the deive is about 4 X 1 X 0.65in big. There is a 3d printed case for holding the PCB. The PCB is a 2 layered boared with 0.15mm trace width and spacing. Most componces are are SMD (excpeted the buttons and the displays). If you do decide to make this project you will need to add shielding inside of the case or else the button clicker will randomly count up, reset, or count down. All the electronics was done using KiCad and the case was made using FreeCAD (all desing files are in the repo if you want to make modications). 

# Images
![IMG_20230215_203119](https://github.com/sam-was-here/button-clicker/assets/102840190/f6737c02-d3ff-409c-bf5a-29d78b7f556e)
![IMG_20230215_175122](https://github.com/sam-was-here/button-clicker/assets/102840190/d61c9d7f-647d-45af-8ad3-b09db66a89a1)
![IMG_20230215_203104](https://github.com/sam-was-here/button-clicker/assets/102840190/5f10ca7f-78ca-465b-a5b3-b0a1b61fc737)
![IMG_20230215_204520](https://github.com/sam-was-here/button-clicker/assets/102840190/2165c615-4cdc-498e-aa29-04d5a3c152f4)
![IMG_20230215_204531](https://github.com/sam-was-here/button-clicker/assets/102840190/05e833c8-f731-47f1-ad7b-6e20aca46a87)

# BOM
BT1: 3034TR - cr2032 batter holder - https://www.digikey.com/short/wqhf8fbf
C1-C11: 0603 0.1uF ceramic cap - bypass cap - 
D1: SOD-523 - crowbar diode for reverse polarity protection - 
D2-D5: SMA  - TVS diode - https://mou.sr/43r05RL
R1-R5: 0603 100k 5% resistor - buttons pull up/down resistors and debounceing
R6-R47: 0603 1k 5% resistor - led current limiting resistors
SW1: THT tack switch right angle - button that its clicks are counted - https://mou.sr/42t1Exi
SW2: THT tack switch right angle - button to light up display - https://mou.sr/42t1Exi
SW3: SMD tack switch - reset button - https://mou.sr/3oV6upt
U1: SOT-23 (5) 74LVC1G17 - Single Schmitt-Trigger Buffer - https://www.digikey.com/short/7bh4nv4q
U2-U4: TSSOP-16 74HC390 - DUAL DECADE RPL COUNTR - https://mou.sr/3katv4U
U5-U10: TSSOP-16 74HC4511 - BCD-to-7 Segment - https://www.digikey.com/short/bz3pz8r9
U11-U16: INND-TS30RCB - red 7 segment display - https://www.digikey.com/short/40qw31cv
# Schematic
![button-clicker.pdf](button-clicker.pdf)


