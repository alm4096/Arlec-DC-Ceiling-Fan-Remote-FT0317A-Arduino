# Arlec DC Ceiling Fan Remote FT0317A Arduino
Bare bones code to control the Arlec Grid Connect Ceiling Fan (replacing the 433MHz remote) from an Arduino using the MX-RM-5V a cheap chinese 433MHz transmitter or similar. Take note that pin D11 is used to send the data. The circuit is as simple as it sounds. I used an Arduino Nano ATMega168, the code in untested on other Arduinos (the delay 34ms could be an issue).

I have had to modify the RC-Switch library to accept 40bit code and a sync pulse. If you use the standard RC-Switch library you will have issues compiling. Simply copy the RC-Switch library into your Arduino\libraries folder under your Documents folder (Windows).

Make sure you copy the example, you need to send the 'b' code then the 'c' code.

NOTE: This remote is used on a number of other ceiling fans, if your remote looks the same give this sketch a go. The OEM is Shenzhen Funpower and szfunpower is written on the PCB of the remote. 

![FT0317A image](FT0317A.png?raw=true "FT0317A Image")
![Circuit image](Circuit.jpg?raw=true "Circuit Image")
