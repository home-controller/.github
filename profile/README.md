## Code used for home automation.

### Index:
* [__arduino-store__.](https://github.com/home-controller/arduino-store) *Store data records permanently. Only EEPROM for now but planning to add more.(uses EEPROM.h, ui_io.h, defs.h)*  
* [__1wire_io__.](https://github.com/home-controller/1wire_io) *For reading and setting 1wire IO eg. DS2413, DS2408, DS2405, 3A 2100H etc. (uses OneWire.h)*
*  [___serial IO.___](https://github.com/home-controller/ui_io) *some helpers for serial IO mostly macros* 
   * [___cat serial IO.___](https://github.com/home-controller/ui_io/tree/master/examples/tty_colours) *How to use cat to display serial input and out put from the Ardunio so it shows colour etc as the Ardunio built in serial console lacks VT100 suport*

 ###  Using cat to read from serial on linux

The Arduino built in console don't support colour or other VT100 codes so  if you need one does etc this can be handy.
 
On my computer using the standard bash console works to read the serial output from an Ardunio pluged into a USB port.

I am using Linux with a KDE desktop and using Konsole as the terminal.

As an example with my Nano board plugged in on /dev/ttyUSB0 and the serial speed set to 38400 the following bash commands work:

stty -F /dev/ttyUSB0 38400 raw
cat /dev/ttyUSB0

cat returned after each line when I had 2 arduinos 1 each on /dev/ttyUSB0 and /dev/ttyUSB1 buf tail still worked.

tail -f /dev/

I can also use the cat command in another bash terminal to type to the Nano.
