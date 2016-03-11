PX4Flow Board Firmware
====

This is a working copy of https://github.com/PX4/Flow/tree/klt_flow2

Main changes:

  - Fixed bug is inc/utils.h file. Changed itoa to gfc_itoa to compile.
  - New Parameters set in src/settings.c.

Tested and working with Ubuntu 14.04LTS.

Original Project:
http://pixhawk.org

Requirements
==
- Toolchain installation: visit for http://pixhawk.org/dev/px4flow Dev guide / toolchain installation 

Compilation and Flashing
==

To build, run:

  make

To flash via the PX4 bootloader (first run this command, then connect the board):

  make upload-usb

Sensor Settings
==
Change sensor settings in file: Flow-klt_flow2/src/settings.c

WARNINGS
==
Firmware not compatible with newest versions of QGroundControl software.  
