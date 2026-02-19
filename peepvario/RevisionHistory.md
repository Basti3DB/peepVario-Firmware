# Revision History

# Peep Vario Firmware

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
* try fix: MAC-OS usb mode

###  	v1.1.3:
* add tone curve presets
* add audio threshold presets
* add tone feedback when usb is connected
* change accel scale to 8g and gyro to 500dps (was clipping before)
* add Kalman accel bias estimate
* add Kalman adaptive accel noise scale
* tune Kalman parameters
* remove adaptive scaling in orientation filter
* adapt Kalman to use different sensor data rates in future

###  	v1.2.1:
* Implemented a fully ESKF for Sensor fusion
* usb on macos still buggy

###  	v1.2.3:
* changed oconfig file save format in flash (now binary)
* removed unused kalman parameters
* Tuned ESKF parameters
* Add g-force to XCTOD protocol
* add ble webconfig support
* ble firmwareupdate

# BOOTLOADER:

### v1.0.0:
* initial version

###  	v1.0.1:
* USB connection check + Button press check

###  	v1.0.2:
* ONLY works with Firmware >v112
* upgrade max size to 18KB
* temp. fix: end of update file detection

###  	v1.1.0:
* add firmware update via BLE

