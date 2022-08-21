# 74XX-Defined-Radio
This is a PCB design for the 74XX defined radio receiver which was on hackaday.com

Here is the link to the original article.  

https://hackaday.com/2021/04/19/a-superheterodyne-receiver-with-a-74xx-twist/

I made an arduino shield for it.  The original design has been modified as such:

1. I added a bandwidth switch to select the IF bandwidth for 3000 Hz and 1800 Hz.  I would like the narrow band to be a
   sharper for CW, but decided to stop fooling with the simulation and go build a radio.
   
2.  The IF is not at 100 kHz as the original, and the original was not at that frequency either.  It does not really
   matter as the LO will take care of it.
   
3.  I added an Adafruit PLL module for the LO.  This will be under software control by the Arduino.  The software will
   written so as to back out the IF frequency so that when one selects 10.000 MHz, that is what you will get.
   
4.  Because the Adafruit module has multiple outputs, I added one for a beat frequency osicllator (BFO).

I have not yet built this radio, so, caveat emptor, or Your Mileage may Vary.  I also have not written the Arduino
code, but I am sure the examples on the Adafruit site are a good start.  If anyone reading this wishes to volunteer
to take a stab at it, be my guest.

As of this writing all parts are available for purchase.  The antenna connector is at Arrow Electronics. If you want one
stop shopping, this part from Wurth may fit, but the holes may be a little tight.  691137710002 is the.

I may be reached at KA1CRV@arrl.net
