avoccado-avr-pcb
================

Schematics and PCB layout for the avoccado-avr controller.

![IMG board screenshot](20140912-A1-gerber-files/rendered/ScreenShot_6.png)

USB bootloader option to update the firmware if the 68R resistors are populated. The USB data lines connect to D2 and D7.
There is a 2K pullup to 3.3V at the D- USB data line, no zener diodes to limit the voltage at the data lines because the MCU runs at USB compliant 3.3V VCC, see vUSB recommendations here: http://vusb.wikidot.com/hardware
