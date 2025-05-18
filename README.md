# DIY Voice Assistant

Disclaimer: I have not yet finished building this, therefore there may be slight issues with the models.

I set out to build a voice assistant that had a small footprint (allowing it to fit easily in any space), A high quality speaker (for voice clarity and music) and a high power processor (to allow for on device speech processing allowing audio to stay on device). My design consists of a cylinder like shape with a visible speaker at the top. There is a status LED strip in a ring at the bottom to show the devices status and give a visual indicator of the device being activated. There are a ring of holes near the base to allow for sound to travel into the microphones. The holes at the bottom also make the design act as a transmission line speaker giving better bass.

![image.png](/CAD/Images/image-7.png) ![image-6.png](/CAD/Images/image-6.png)

## How to Build

- Print the model. The casing is best printed in a single peice using PVA or BVOH supports on a large printer. On smaller printers, it can be split into 2 and printed with standard tree supports.
- Assemble electroncs. First install the HAT on the Raspberry Pi. Splice a USB-C cable for power input to the Raspberry PI and solder to the power output on the buck converter. Splice an aux cable for sound output and wire to the amplifier audio input terminals. Wire the barell jack directly to the amplifier power input and the buck converter input. Wire the buck converter output to the LED strip. Connect the LED strip to pin 12 on the raspberry pi. 
- Wrap the LED strip around the indented area (green in the above render) of the unit adhering it with the built in adhesive. Run the end through the slot so wire to the internal electronics. Place an adhesive diffuser ontop (optional)/
- Install an SD card in the Raspberry Pi preloaded with any linux based operating system. Ensure it is connected to wifi and SSH is enabled so it can be programmed from within the unit.
- Install all electronics. Start by screwing in the raspberry pi and amplifier boards. Glue in the barell jack. Screw in the buck converter and finally screw in the speaker.  
- Plug it in and voila!

## BOM (Excluding fillament for printing)

| Part name                        | GBP Price | USD Price | Use                   | URL                                                                 |
| -------------------------------- | --------- | --------- | --------------------- | ------------------------------------------------------------------- |
| Dayton Audio PS95                | £42.32    |           | Play the audio output | https://www.ebay.co.uk/itm/146374373328                             |
| 15W 16V Digital Amplifier Module | £1.19     |           | Drive Speaker         | https://www.aliexpress.com/item/4000124520883.html                  |
| Raspberry Pi 5                   | £45.26    |           | Processor             | https://thepihut.com/products/raspberry-pi-5?variant=43878483198147 |
| WS2812 LED strip                 | £5.59     |           | Shows device state    | https://a.aliexpress.com/_EJAJOKw                                   |
| Power supply                     | £7.19     |           | Power input           | https://www.aliexpress.com/item/33059222345.html                    |
| buck converter                   | £3.58     |           | 5v power              | https://www.aliexpress.com/item/1005007617487215.html               |
| Microphone Hat                   | £6.09     |           | Take audio input      | https://www.aliexpress.com/item/32902300949.html                    |
| Barrel jack                      | £0.72     |           | Take power input      | https://www.aliexpress.com/item/4001206395694.html                  |
| Total                            | £110.94   | $147.33   |                       |                                                                     |

