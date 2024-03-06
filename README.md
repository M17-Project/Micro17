[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

# Micro17
M17 baseband processor board - OpenRTX on a Module.

## What is it?
An M17 baseband processor in a small form factor. Similar to
[Module17](https://github.com/M17-Project/Module_17) but much more compact.

## AT command set
|Interface setting|Command|Valid values|
|-----------------|-------|------------|
|Invert TX baseband|AT+INVTX|0/1|
|Invert RX baseband|AT+INVRX|0/1|
|TX baseband level|AT+TXLVL|0..255|
|RX baseband gain|AT+RXLVL|0..255|

|M17-specific setting|Command|Valid values|
|--------------------|-------|------------|
|Source callsign (SRC)|AT+SRC|up to 8 characters long string, eg. "N0CALL"|
|Destination callsign (DST)|AT+DST|up to 8 characters long string, eg. "ALL"|
|Transmit CAN|AT+TXCAN|0..15|
|Receive CAN|AT+RXCAN|0..15|
|Encryption|AT+ENCR|0/1/2|
|M17 `META` field|AT+META|raw 112-bit (14-byte) field|

|M17 packet mode|Command|Valid values|
|---------------|-------|------------|
|Transmit message|AT+MSG| string, eg. "Hello world!"|

## License
This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg
