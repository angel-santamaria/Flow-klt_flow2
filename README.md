## PX4Flow Board Firmware

This is a working copy of https://github.com/PX4/Flow/tree/klt_flow2

Main changes:

  - Fixed bug in inc/utils.h file (changed itoa to gfc_itoa).
  - New Parameters set in src/settings.c.

Tested and working with Ubuntu 16.04LTS.

Prepared to work with ROS package: https://github.com/cvg/px-ros-pkg

Original Project: http://pixhawk.org

#### Requirements

* User rights to groupd **dialout**: `sudo adduser <user_name> dialout` 

* Toolchain installation: `sudo apt-get install gcc-arm-none-eabi`

#### Compilation and Flashing

* To **build**, go into the firmware folder and run:

  `make`

* **Unplug** your PX4Flow device.

* Flash via the PX4 bootloader (**first run the following command and then connect the device**):

  `make upload-usb`

#### Sensor Settings

Change sensor settings in file: Flow-klt_flow2/src/settings.c

#### WARNINGS

**Firmware NOT COMPATIBLE with newest versions of QGroundControl software.**  
