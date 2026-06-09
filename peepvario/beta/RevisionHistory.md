# Peep Vario beta Firmware

### v1.0.0 _ 1:
* 
### v1.2.1 _ UART_BINARY:
* 
### v1.2.6 _ 2:
* 
### v1.2.6 _ ESKF_fasterBiasEstimate:
* 
### v1.2.11 _ lowPower_bugTakeoff:
* 
### v1.2.12 _ HWoutputs:
* 
### v1.2.12 _ HWoutputs_3:
* 
### v1.2.13 _ HWoutputs_2:
* 
### v1.2.13 _ ringubffer:
* 

### v1.3.4 _ 1:
* 
### v1.3.4 _ 2:
* fix auto revision. Focused on CI automation.

### v1.3.4 _ 3:
* add audio volume LOW. Focused on application behavior, configuration handling, task scheduling and runtime behavior.

### v1.3.4 _ 4:
* fix landing thresholds, adjust eskf. Focused on sensor fusion and processing, task scheduling and runtime behavior.

### v1.3.4 _ 5:
- add BLE config capabilities
- change tonecurve standart to xc tracer default
- edit auto obeta commit - include all commit msg of push

### v1.3.4 _ 6:
- change tonecurve preset2 name to sniffer
- refactor configserializer
- remove igc key
- lower battery beeps f
- even lower battery beeps f

### v1.3.4 _ 7:
- add audio volume control with >1 sec long press

### v1.3.4 _ 8:
- fix production build

### v1.3.4 _ 9:
- fix test framework
- manual takeoff detection double press, tripple press is calibration

### v1.3.4 _ 10:
- set low volume pwm duty to 1

### v1.3.4 _ 11:
- change default othresholdpreset to standard

### v1.3.4 _ 12:
- add logo
- add baro pseudo vertical speed
- tune eskf accel bias estimate

### v1.3.4 _ 13:
- tune eskf gyro bias estimate

### v1.3.4 _ 14:
- tune eskf

### v1.3.4 _ 15:
- fix takeoff threshold range

### v1.3.4 _ 16:
- change order of presets

### v1.3.5 _ 1:
- VERSION 1 3 5, Implement new Piezo driver Add proper LaTeX Manuals
- add new configparameter: userStorage
- new audio output not working... remove some overhead to fit in flash

### v1.3.5 _ 2:
- fix system.userstorrage

### v1.3.5 _ 3:
- Ignore button long press on startup
- Better error handling (more retries) - auto shutdown
- fix error auto shutdown
- more toleroant landing detection

### v1.3.5 _ 4:
- NOT WORKING
- bugfix: volume change with device was not saving
- better landing, better eskf

### v1.3.5 _ 5:
- NOT WORKING
- adjust SNIFFER preset

### v1.3.5 _ 6:
- restore working eskf params
- try Audio PWM Sine
- add nice built statistics

### v1.3.5 _ 7:
- new eskf parameters

### v1.3.5 _ 8:
- add simulation run as TestCase
- fix simulation again
- new eskf parameters

### v1.3.5 _ 9:
- add tripple press for manual landing
- and fix simulation test case

### v1.3.5 _ 10:
- same as (9)
- test website cache refresh

### v1.3.5 _ 11:
- new eskf parameters

### v1.3.5 _ 12:
- new eskf parameters; fixed landing detection (10s)

### v1.3.5 _ 13:
- new button gestures: Double press: Changes volume. Triple press: Triggers manual takeoff (before flight) or manual landing (during flight). Long press (1s): Enters heading lock mode (with a short beep after 1s for feedback). Single short press when heading lock active: Exits heading lock.

### v1.4.1 _ 1:
- VERSION 1 4 0
- VERSION 1 4 1

### v1.4.1 _ 2:
- try different Audio modulation

### v1.4.1 _ 3:
- work on liftair user manual
- try different Audio modulation 2
- FIX: use new tone after threshold is reached

### v1.4.1 _ 4:
- fix: beep mixup of fast buttonpresses

### v1.4.1 _ 5:
- change volume name of usb device
- BL version 1 3 0 - new usb volume name
- huge audio improovements
- add landing beep
- bugfix: landing detection state transition

### v1.4.1 _ 6:
- add separate 1s button press confirmation beep
- BL verison 1 4 0 audio improvements
- 1s button press, shorter play time

### v1.5.1 _ 1:
- Version 1 5 0 -> 1 5 1 now working
- try new eskf parameters (higher bias estimate)

### v1.5.1 _ 2:
- More tolerant landing detection
- update github pages

### v1.5.1 _ 3:
- try new eskf parameters (changed expected noise)

### v1.5.1 _ 4:
- try new eskf parameters (lower baro noise)

### v1.5.1 _ 5:
- intital setup for LiftAir_zero_v2
- add to cmake

### v1.5.1 _ 6:
- add EEPROM to HardwareFactory
- wire IGC log to SD card
- add SW update flow diagram
- add UML
- fix uml compiler
- add new pins to Liftairzerov2 product
- change uml

### v1.5.1 _ 7:
- update uml
- add heartbeat to bootloaderupdater
- refactor Bootloader updater make all paths relative
- apply same blu to liftairzerov2
- refactor Production Test
- add eeprom to test
- add simulation outputs to git ignore
- Add UTC timestamp to SD igc log
- make dataflow uml
- tune ESKF

### v1.5.1 _ 8:
- create interface class for bluetooth device
- remove additional audio velocity filter, which caused delay
- lower direct fire threshold

### v1.5.1 _ 9:
- add IGC log forwarding via ble
- add nrf ble module implementation to liftair zero v2
- Merge branch 'main' of https://github.com/Basti3DB/peepVario-dev

### v1.5.1 _ 10:
- fix bootloader built issue
- fix Production test build issues
- fix test run
- add LZV2 to beta firmware upload
- also update manual upload, also only uplaod if tests run clean

### v1.5.1 _ 11:
- add IGC log forwarding via ble
- add nrf ble module implementation to liftair zero v2
- ble add deticated command protocol set
- Merge branch 'main' of https://github.com/Basti3DB/peepVario-dev
- fix bootloader built issue
- fix Production test build issues
- fix test run
- add LZV2 to beta firmware upload
- also update manual upload, also only uplaod if tests run clean
- fix target folder

### v1.5.1 _ 12:
- remove unwanted default ble telemetry data
- Change hardcoded MagnetSensor orientation "flip"
- move BootloaderUpdater into LiftAirzeroV2 product (instead of separate FW needed)
- lower preamble pusle (nicer audio)
- Tune ESKF
- add experimental touch detection
