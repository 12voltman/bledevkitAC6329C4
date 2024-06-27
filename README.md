# Dev board for the AC6329C4 from JieLi Tech
Able to be found for an astounding $0.25 in quantity [here](https://www.lcsc.com/product-detail/Microcontroller-Units-MCUs-MPUs-SOCs_JieLi-Tech-AC6329C4_C5440081.html), the AC6329C4 is a promising chip for ultra low cost BLE devices.  
Some of the cool features of this chip:  
- Integrated battery charger
- Integrated LDO for powering peripherals
- BLE 5.3 (may support further with new firmware)
- Full-speed USB OTG with built-in bootloader (needs weird trigger to enter DFU)
- 3 UARTs
- 1 I<sup>2</sup>C
- RTC
- 10-bit ADC w/ 6 channels
## Dev board features
This chip has some oddities around the bootloader, which needs a very specific bit pattern to be presented on the USB lines to enter DFU mode.  To enter DFU mode, I added an ATTINY microcontroller and a USB isolation switch, which also lets you use the USB pins as extra IOs if desired.  
