# FlipperZeroESPexpansion
Flipper Zero ESP-01s Wifi Expansion Module
This module supports the SequoiaSan Wifi Scanner Plugin and the Timmotools ESP8266 Wifi Deauther Plugin
![Screenshot_1](https://user-images.githubusercontent.com/35648759/193376133-197d9094-1b14-46ee-a3b7-923488f23fe3.png)

# Firstly a warning. DO NOT HOTPLUG ANY MODULES. Please turn the flipper off before inserting.

Purchase here: (https://www.tindie.com/products/speexvocon/flipper-zero-esp-01s-module/)

# Parts and Assembly

This module is low on parts count so they should be easily sourced. 

The heart of this is the ESP-01s. Note this has to be the 01s variant because the other, older module requires pull-up resistors for programming. 
You can readily get these on amazon, or aliexpress. Note that sourcing parts from aliexpress will take longer, but is generally cheaper. 

Here are some links for the module. 

Aliexpress: https://www.aliexpress.us/item/2251801851082242.html

Amazon: https://www.amazon.com/DIYmall-ESP8266-ESP-01S-Serial-Transceiver/dp/B00O34AGSU/

The pushbuttons are a fairly common through-hole type. They are somewhat optional, because you could use tweezers or a jumper wire to short the pins for programming or reset. 

I recommend the ebay link if you are in the States. 

eBay: https://www.ebay.com/itm/254595728722

Amazon: https://www.amazon.com/dp/B008DS188Y

Aliexpress: https://www.aliexpress.us/item/2255799843766580.html

The capacitor is optional but if you have issues, you can solder in a 10uf cap that will fit. Mind the + leg as indicated on the pcb. I used a tantalum cap in the reference design. 

Headers. I used the run of the mill vertical male headers. You need one row of 10. 

Amazon: https://www.amazon.com/MCIGICM-Header-2-45mm-Arduino-Connector/dp/B07PKKY8BX/

Aliexpress: https://www.aliexpress.us/item/2255800671070360.html

eBay: https://www.ebay.com/itm/394043494907

If you want to use the flipper as a bulk ESP-01s programmer, I recommend a 2x4 pin socket for the modules. 

As for the PCB, you may be able order from me, I might have some left. Otherwise, you can get them cheaply by uploading the pcb gerber zip file in this repo to jlcpcb.com using default settings and lowest shipping rate, it would cost roughly $5.47 for 5 boards and would take a couple weeks as they come from China. For convenience and speed, I may put the PCBs up on Tindie. Just let me know on twitter or discord and I can direct you to the best resource. 


## Programming the module

Programming the module can be done via webflasher [here](https://speexvocon.github.io)

To put the module into program mode:
	
		First, hold down the PrgEN button.
		While holding the PrgEN button, press the reset button.
		Let go of both. If you did this correctly, you should be in program mode.
		
To program with the flipper:

	Goto GPIO
	Select USB-UART bridge
	Hit the left arrow buttong to enter CONFIG
	Set USB Channel to 1
	Baudrate to Host
	Uart Pins 13,14
	RTS/DTR to none
	hit the back button
	Plug into the computer
	Two serial ports should show. Select the one with the highest number, (for me it showed 14 and 16, so I chose 16)
	EDIT: this may not be the case, so try one port, if that doesn't work, try the other.
	
Now you should be ready for the webflasher (linked above)
