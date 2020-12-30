# Level2_Makerfair2019_robot
The code used in the 2019 [Makerfair](https://luxembourg.makerfaire.com) competitionfrom the team Code Club/Level2

The actual Hardware:
* Makeblock Ultimate 2.0
* PN 532 (V1 other versions should work fine to but the pinout might be different)

## Software

We used the firmware for the MegaPi we got from the [MakeBlock](https://github.com/Makeblock-official/Makeblock-Libraries/blob/master/examples/Firmware_for_MegaPi/Firmware_for_MegaPi.ino) repo.

The .ino file can be opened in the Arduino IDE.
You also need to install the PN_532 library for the NFC capability.
To do this go to Sketch -> Include Library -> Manage Libraries  There you search for PN 532 and install the library.

Next you need to select the right Board and Port for the upload.
Connect your bot to th ecomputer via the USB cord, make sure it's on and choose the correct port.
* Under Tools -> Port: 
We usedd the Arduino Mega ADK (ALthoug other probably work to)
* Under Tools -> Board: -> Arduino Mega ADK

Now you should be good to go on the software side.
Upload the file using the Upload Button or Sketch -> Upload

## Hardware

The PN_532 is directly connected to the MegaPi via the SPI pins.
* The MOSI pin from the PN_532 gets connected to the MOSI pin of the MegaPi (SPI pin4)
* The SS pin from the PN_532 to the Pin A12
* The MISO pin to MISO pin (Pin 1)
* The SCK to SCK (pin 3)
* The rst to RESET (pin 5)
* The 5V pin gets connected to the +Vcc pin (pin2)
* Gnd gets connected to Gnd (pin 6)
![Board view](https://github.com/felixgasiaux/Level2_Makerfair2019_robot/blob/master/Images/MakeBlock-MegaPi-ports_make_it.png)
Image provided from [Makeit](https://www.makeit.lu)
![PN_532](https://github.com/felixgasiaux/Level2_Makerfair2019_robot/blob/master/Images/fritzing_schematic_TVQHEt1w6d.png)


## Use 

Simply open the 
