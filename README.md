
[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

# Micro17
M17 baseband processor board - OpenRTX on a Module.
![Micro17 connected to an ICOM radio.](/icom_ICF3_4_5_6XXX/icom_micro17_board1.jpg)

## What is this?
Micro17 is an integrated implementation of Module17. Its PCB design is radio-dependent, but the general schematic is quite close to Module17. 
For more info about M17 and Module17, please checkout [M17's Website](https://m17project.org/) and [Module17's Github](https://github.com/M17-Project/Module_17) .

## Supported radios - variants
|Brand/Models|Status|
|-----------------|-------|
|[Generic (for all radios, can be used with modwires)](/generic/)|Hardware design WIP|
|[ICOM IC-F3XXX/4XXX/5XXX/6XXX](/icom_ICF3_4_5_6XXX/)|PoC OK, hardware design finished, fw WIP|
|[Motorola Waris (GM340/360/etc.)](/moto_waris/)|PoC OK, hardware design WIP|

## Adding support for other models
Do you have a radio that could be compatible with such an implementation? 
Any header (or ribbon cable connector) inside with the following pins can be used:
 - Flat audio in/out
 - Micro/Speaker lines
 - PTT in/out
 - Power supply 
 - (nice to have) command lines for interfacing with the radio's CPU
 
Very often, commercial radios with a scrambling board option have such lines inside. A Module17 modem is a perfect base to test a Proof of Concept before starting hardware design.
When creating a new variant of Micro17, you can use the "generic" variant as a working base, just copy and rename that folder.

## License
This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg

