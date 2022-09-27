# FlipperZeroESPexpansion
 Flipper Zero ESP-01s Wifi Expansion Module
![20220926_133545](https://user-images.githubusercontent.com/35648759/192592396-be1f0fed-1ad8-4db6-abda-740442b20c4f.jpg)

# Firstly a warning. DO NOT HOTPLUG ANY MODULES. Please turn the flipper off before inserting.

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
