## Code used for home automation.

### Index:
* [__arduino-store__.](https://github.com/home-controller/arduino-store) *Store data records permanently. Only EEPROM for now but planning to add more.(uses EEPROM.h, ui_io.h, defs.h)*  
* [__1wire_io__.](https://github.com/home-controller/1wire_io) *For reading and setting 1wire IO eg. DS2413, DS2408, DS2405, 3A 2100H etc. (uses OneWire.h)*
*  [___serial IO.___](https://github.com/home-controller/ui_io) *some helpers for serial IO mostly macros* 
   * [___cat serial IO.___](https://github.com/home-controller/ui_io/tree/master/examples/tty_colours) *How to use cat to display serial input and output from the Arduino so it shows colour etc as the Ardunio built-in serial console lacks VT100 support*
*  [___Home Network___](https://github.com/home-controller/homeauto_network/) *A simple Network to work on MCU GPIO pins, it uses 1 or 2 pins depending on if you want more robust with extra hardware(resistors and transistor at simplest) or direct IO pin connection. This can back-feed unpowered units and hence disable the entire network if 1 unit is unpowered for example.*
