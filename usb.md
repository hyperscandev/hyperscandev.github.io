# USB Access

## Theory
The USB port on the back of the Hyperscan doesn't work out of the box. A common theory is that they already had chosen the PSU and the feature wasn't going to be utilized.
To follow the USB specifications, the power supply needs to provide a clean 500mA current at 5V. I don't think the power supply was able to do that with all the other devices
connected.

### TLDR
1) There's a GPIO register that needs to be turned on that provides power to the USB port.
2) There's not enough power to run the USB port, which is probably why 1 is off.

## Facts
You can power the USB port in order to connect a USB flash drive and run homebrew.

### Items Needed
[USB Cable](https://www.amazon.com/dp/B01AYO9YWQ)  
[Y Splitter](https://www.amazon.com/dp/B085BJRZN2)  
[Power Source](https://www.amazon.com/dp/B0CHVTVS1L)  
[Flash Drive](https://www.amazon.com/dp/B07K82N8NS) - Any will work as long as it's formatted with a Fat32 partition.  

### Steps
1) Insert the USB Flash Drive into your PC and format it using the default settings and FAT32 as the file system.
2) Download [usbfiles.zip](https://github.com/hyperscandev/hyperscandev.github.io/files/15192846/usbfiles.zip) and unzip them somewhere you can find them easily.
3) Copy the files into your USB Flash Drive.
4) Remove the USB Flash Drive from your PC.
5) Insert the USB Flash Drive into one of the 2 female ends of the Y Splitter.
6) Insert the male end of the Y Splitter into the USB port on the back of the Hyperscan.
7) Insert one end of the USB cable into the other female end of the Y Splitter.
8) Insert the other end of the USB cable into a power source.
9) Power on the Hyperscan.

If you followed the instructions, when you turn on the Hyperscan you should see the USB Loader.

### Troubleshooting
* All the connections are secure.
* The power source is sufficient.
* The USB Loader files are at the root of the USB Flash Drive.
* The USB Flash Drive is formatted with FAT32 as the file system.
