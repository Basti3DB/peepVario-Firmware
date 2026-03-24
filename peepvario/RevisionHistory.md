# Revision History
R1

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

###  	v1.2.4:
* add shutdown via ble
* fix website connect on first try
* disabled: load default config all the time

###  	v1.2.5:
* read serial number from OTP (one time programmable)
* read hardware revision from OTP (one time programmable)
* Send both via ble to website

###  	v1.2.6:
* tune ESKF
* better audio output
* remove debug values in config file
* fix vario run after website disconnect
* add watchdog supervison
* add beep on website connect

###  	v1.2.7:
* add tone simulator via website
* fix tonecurve save 
* fix audio (sinkrates)
* fix ble name

###  	v1.2.8:
* add auto-shutdown (after 15 minutes)
* tune ESKF
* add Bootloader version to config
* fix landing detection

###  	v1.2.9:
* fix battery use real LiPo curve
* change BLE name to "...-cfg" -> without for XCTrack
* fix Bluetooth startup time
* fix default tone profile

###  	v1.2.10:
* better landing & takeoff detection
* add Bluetooth auto shutdown after 5 minutes to save power
* add BLE config command: GET SN

###  	v1.2.11:
* BUG: takeoff detection not working
* reduce battery read to 10 minutes
* save and load bias estimates of eskf

###  	v1.2.12:
* Tripple press = manual takeoff detection
* change default takeoff threshold to 2m/s
* fix tonepoint parser
* fix eskf bias save

###  	v1.2.13:
* bugfix: audio queue delay
* tune ESKF parameters
* new tonecurve defaults

###  	v1.3.0:
* ESKF use mag sensor
* new startup/shutdown melody
* new calibration sucess beep
* bugfix: config parsing case insensitive

###  	v1.3.1:
* add blinky LED
* add flight statistics
* fix auto shutdown

