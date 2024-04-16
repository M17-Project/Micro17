# Micro17 - IC-F3/4/5/6X6X
Variant of Micro17 for ICOM IC-F commercial radios.
![Micro17 connected to an ICOM radio.](/icom_ICF3_4_5_6XXX/icom_micro17_board2.jpg)
## Flashing OpenRTX
WIP - ST-Link needed

## Installing Micro17 inside the radio
A Youtube video guide is planned soon:tm:. 
### Mobiles
Getting inside mobile IC-F5X6X/6X6X is quite straightforward: four screws will allow you to pop the bottom cover off. 
You'll need to cut/solder the following bridges:
* Cut "K", "A", "B" and "C"
* Solder/bridge "L"

You can then install Micro17 in the J1 slot. 
![Micro17 connected to an ICOM radio.](/icom_ICF3_4_5_6XXX/icom_micro17_board1.jpg)
### Handsets
Opening a handset is a bit more tricky. You'll need to remove the two knobs, unscrew the antenna nut (either using thin needle-nose pliers or the appropriate tool. Be careful as it might be glued, some light blasting with a heat gun might be needed) and the two bottom screws behind the battery. 
The following bridges will have to be changed: 
* Cut "CP2", "MIC", "AFOUT" and "PTT" 
* Solder/bridge  "CP3"
You can then install Micro17 in the J1 slot.

## Configuring Micro17
As this module is embedded inside the radio, configuration is pulled from the radio's "codeplug". This is still heavily WIP, but it's planned to use the internal command protocol one the details get figured out. 

## Wiring details
This variant is based on the experiments documented [here](https://wiki.m17project.org/icf5060_3060). 
The internal J1 connector breaks out all necessary pins.
| **Module17 equivalent Pins**          | **J1 connector**                                                                                                           |
|----------------------------|--------------------------------------------------------------------------------------------------------------------------------|
| GND (DB9 - pin 8)          | Pin 2, 17 or 39 - GND                                                                                                          |
| +12V/+8V (DB9 - pin 9)         | Pin 37 - VCC                                                                                                                   |
| RX (DB9 - pin 6)           | Pin 31 - DISC                                                                                                                  |
| TX (DB9 - pin 2)           | Pin 13 - SIGO                                                                                                                  |
| PTT_OUT (DB9 - pin 5)      | Pin 4 - PTTO (Add a 1K pullup to 5V - pin 38!)                                                                                 |
| AF_OUT (pot middle pin)    | Pin 30 - AFOUT                                                                                                                 |
| MIC_IN (jack's middle pin) | Pin 7 - MCIN                                                                                                                   |
| PTT_IN (jack's last pin)   | Pin 3 - PTTIN (Through a resistive divider: two 2.7k resistors in series between pins 2 and 3, wire to Module17 in the middle) |



