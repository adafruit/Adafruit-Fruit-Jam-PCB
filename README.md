## Adafruit Fruit Jam - Mini RP2350 Computer PCB

<a href="http://www.adafruit.com/products/6200"><img src="assets/6200.jpg?raw=true" width="500px"><br/>
Click here to purchase one from the Adafruit shop</a>

PCB files for the Adafruit Fruit Jam - Mini RP2350 Computer. 

Format is EagleCAD schematic and board layout
* https://www.adafruit.com/product/6200

### Description

We were catching up on a recent hackaday hackchat with eben upton and learned some fun facts: such as the DVI hack for the RP2040 was inspired by a device called the IchigoJam. we remember reading about this back when it was an LPC1114, now it uses an RP2040. well, we're wrapping up the Metro RP2350 and lately we've been joking around that with DVI output and USB Host support via bit-banged PIO, you could sorta build a little stand-alone computer.

Well, one pear-green-tea-fueled-afternoon later we tried our hand at designing a 'credit card sized' computer - that's 3.375" x 2.125", about the same size as a business card and turns out there's even a standard named for it: ISO/IEC 7810 ID-1.

Anyhow, with the extra pins of the QFN-80 RP2350B, we're able to jam a ridonkulous amount of hardware into this shape:

* RP2350B dual 150MHz Cortex M33
* PicoProbe debug port
* 16 MB Flash + 8 MB PSRAM - the PSRAM will help when we want do do things like run emulations that we need to store in fast RAM access, and also let us use the main SRAM as the DVI video buffer.
* USB type C for bootloading/USB client
* Micro SD card with SPI or SDIO
* DVI output on the HSTX port
* I2S stereo headphone + mono speaker via the TLV320DAC3100
* 2-port USB type A hub for both keyboard and mouse or game controllers
* Chunky on-off switch
* Stemma QT I2C
* Stemma classic JST 3-pin
* 5x NeoPixels
* 3x tactile switches
* 16-pin socket header with 10 A/D GPIO + 5V/3V/GND power pins.

What should we try running on this hardware when we get the PCBs back and assembled? we're pretty sure it can run DOOM... should that be first? :) we also need a name, right now we're just calling it Fruit Jam since its inspired by the IchigoJam project.

### License

Adafruit invests time and resources providing this open source design, please support Adafruit and open-source hardware by purchasing products from [Adafruit](https://www.adafruit.com)!

Designed by Limor Fried/Ladyada for Adafruit Industries.

Creative Commons Attribution/Share-Alike, all text above must be included in any redistribution. 
See license.txt for additional details.
