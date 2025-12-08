# Revision History



### v1.0.0:

* DFU working
* USB configured as: COM
* General structure working, but can be optimized
* Cloud-fly mode: Gyro-YAW
* sometimes boots into error -> just try it a few times



###  	v1.0.1:

* USB configured as: Mass storage
* Show software version in config file



###  	v1.0.2:

* Show also Serial Number in config file
* fixed: baro init error (-> need HW change)
* Bluetooth (BLE) working, supported protocols are: LXWP0, LK8EX1
* fixed: config file read
* Takeoff detection
* Battery monitoring
* Cloud-fly mode: Integrate Roll angle
* Better Vario Tone (no frequency changes during beep)
* fixed: no tone playing before and after button press \& no tone after switching off sound
* 1 Second button hold for power on
* Longer Calibration-window time



###  	v1.0.3:

* Bluetooth: add XCTrack raw temperature
*            change LK8EX1 to send battery percent instead of voltage



###  	v1.0.4:

* Add 3 axis magnet sensor to Sensorfusion -> 9 DOF
* Add landing detection
* always update sw version in config file
* easy import for xc-tracer audio file in config
* fix: MAC-OS usb mode
* fix: no audio (vario) tones while calibrating



### v1.1.0:

* Firmware updates via USB -> drag\&drop
* Add separate Bootloader



###  	v1.1.1:

* -> new bootloader (only bootloader mode when button press <1s \& usb is connected)
* fix: MAC-OS usb mode



###  	v1.1.2:

* ONLY works with Bootloader >v102
* 





BOOTLOADER: 

### v1.0.0:

* initial version



###  	v1.0.1:

* USB connection check + Button press check
* 



###  	v1.0.2:

* upgrade max size to 18KB
* End of update file detection
* 
