Avoccado° PCB layouts and schematics
================

This repository contains the source files of the PCBs for Avoccado° controllers equipped with AVR micro controllers.

![IMG board screenshot](avoccado-alpha-1/20140912-A1-gerber-files/rendered/ScreenShot_6.png)

There are different PCBs, some with more than one revision. Check the commit log for the most recent development version.

 - Alpha 1 (A1): 8/10 mil width/spacing, 2 sided, components on one side, full size rectangular board a la Arduino Nano / Pro Mini with female micro USB 2.0 and LiPo charger
 - Kane: 8/8 mil, small square board without LiPo charger, components on both sides, good as a tiny RX (receiver) node.
 - Yolandi: 8/8 mil, never tested
 - Nora 1: square board, about one square inch, IRQ from NRF24 routed to MCU
 - Nora 2: same as Nora 1 with IRQ from NRF24 and MPU6050 routed to MCU
 
Alpha 1 (A1):
----------------

USB bootloader option to update the firmware if the 68R resistors are populated. The USB data lines connect to D2 and D7.
There is a 2K pullup to 3.3V at the D- USB data line, no zener diodes to limit the voltage at the data lines because the MCU runs at USB compliant 3.3V VCC, see vUSB recommendations here: http://vusb.wikidot.com/hardware

Nora 2
----------------
Notes and ideas: No cinsistent 100 mil grid with all headers at the moment
Plated half holes are nice for SMD piggybacking the hole board. Mind the test points and exposed pads on the bottom.

Test jigs
----------------
Nora 2 test jig is compatible with Nora 1 and Nora 2
