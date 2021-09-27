# Arlec-DC-Ceiling-Fan-Remote-FT0317A-Arduino
Bare bones code to control the Arlec RC212 Wireless Power Point from an Arduino using the MX-RM-5V a cheap chinese 433MHz transmitter or similar. Take note that pin 11 is used to send the data. The circuit is as simple as it sounds.

I have had to modify the RC-Switch library to accept 40bit code and a sync pulse. If you use the standard RC-Switch library you will have issues compiling. Simply copy the RC-Switch library into your Arduino\libraries folder under your Documents folder (Windows).

Make sure you copy the example, you need to send the 'b' code then the 'c' code.

![FT0317A image](FT0317A.png?raw=true "FT0317A Image")
![Circuit image](Circuit.jpg?raw=true "Circuit Image")
