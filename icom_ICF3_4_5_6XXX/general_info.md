# General information on ICOM IC-FXX6X radios
Almost every variation of the IC-FXX6X should be compatible with Micro17. 

## Model numbering
The model number will help you in identifying which version you have.
It is composed of 4 digits and one or more letters.
### First digit
* 5: Mobile VHF
* 6: Mobile UHF
* 3: Handset VHF
* 6: Handset UHF
  
### Second digit
* 0: compatible
* 1: compatible
* 2: __completely different revision, not compatible__

### Third digit
Only 6 is compatible

### Fourth digit
Market segment: 
* 1: USA
* 2: European Market
* 3: General
Be careful as there are US market models (suffix "1") that are 450-520, and others 400-470. I've managed to bring 450 models down to 434MHz, but it makes things quite complicated. Identifying them requires checking the FCC ID in the database, it'll give you the frequency range. 


### Letter suffixes:
* T: 10-key version
* S: for a 4 key version
* D: digital (with an additional UT-126 board for NXDN and dPMR support. Basically the exact same radio with an additional removable board).
A 4-key version can be case-swapped with a 10 key version without issues. The UT-126 is completely unnecessairy for this M17 mod. Removing it might be a good idea to reduce battery usage. 


### Common examples
In UHF, the IC-F6061 mobile is quite common on eBay. If you're in Europe, you might get lucky and score an IC-F6062. For handsets, the IC-F4161DS pops up a lot.

## Programming the radios
Those radios are channelized, and will require you to program your frequencies one way or another. If you're lucky, you'll be able to program it via the front panel [using this procedure](https://sawback.com/wp-content/uploads/2018/11/Icom-Front-Panel-Programming.pdf) (the combination to trigger programming mode is slightly different: P0 and the button above PTT). 
Otherwise, you'll need the cloning software (a quick google search should help you out) and the programming cable:
* For the handsets, you'll need to buy the cable, cheap clones are available on [Aliexpress](https://www.aliexpress.com/item/1005001671445899.html).
* For the mobiles, Aliexpress can also be your friend... You can also make your own cable using an RJ45 connector and a 5V USB-TTL adapter. Pin 2 goes to RXD, Pin 8 to TXD, Pin 7 to GND.
