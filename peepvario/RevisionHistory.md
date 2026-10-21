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

###  	v1.3.2:
* start calibration via website
* change default BLE name to "LiftAir" + SerialNumber

###  	v1.3.3:
* tune ESKF parameters
* tune audio lowpass filter (faster)
* add: high vertical velocity delta overwrite current audio
* BLE: XTOD add 3 - vertical velocity

###  	v1.3.4:
* add: Audio volume mode "LOW"
* add: Audio volume change with >1s press
* better Takeoff & Landing detection
* add: Manual Takeoff overwrite -> double press
* tune ESKF parameters
* new tone presets & correct order
* Reduce battery percentage beep frequency

###  	v1.4.0:
* Vario working well :)
* changed: Button gestures -> read manual
* * double press: Volume change
* * tripple press: manual takeoff/landing
* * 1s long press: enter heading lock
* * short press: exit heading lock
* changed: SNIFFER audio preset
* fix: save volume after changing
* add: Firmware info (release/beta)

###  	v1.5.0:
* huge audio improvements
* add: Audio feedback for landing detection
* fix: double press audio feedback
* fix: tone mixup at new audio tone
* fix: 1s press indication

###  	v1.5.1:
* Sensor algorithmus improvements
* better automatic landing detection
* small audio improvements

###  	v1.5.2:
* add experimental "touch" detection
### v1.5.3:
- setup my new laptop
- move downloaded nrf software to software
- Download NRF ble "firmware"
- add shortcut to vscode ble dir
- v122, new config binary save
- implement BLE firmware for NRF chip
- change ble code so vs can compile it
- add gitignore
- add version to compiled binary
- add ble run and debug setup
- change ble run configs
- fix ble run configs
- fix ble run configs - segger flash tool
- lots of trials to get ble running
- more trials
- configure clangd
- ble things
- ble tests..
- add calibration via ble, lot of tries to get new ble module running
- ble simple test are working
- change ble led pin to 4
- ble blinky kinda working (break once running)
- ble module onow parly woorking
- add vertical velocity to XCTOD
- start implement transparent uart to ble
- more ble things
- adapt to nordic example
- more trials
- AI means it is working
- BLE now showing up, Bootloader disabled
- BLE connectable
- custom UUID and tx working
- dummy XCTOD
- add Nordic Uart Service UUID
- xctrack works, but no updates
- still no updates
- running again, fixed  clearing faults before debug
- really working after merge, but no periodic update
- xctrack works, also periodic sending
- wire transparent uart to NUS, working
- add task so nrf module does run without debugger
- other things
- implement VG6328 at commands clone
- fix hardfault
- fix UART BLE bridge
- VG6328 clone now working
- Merge all built outputs into 1 file
- Refactor source code
- BLE nrf module fw update: fix long writes
- ble add deticated command protocol set
- LiftAirzeroV2 now booting to app
- fix ble msg checksum, add connection LED (green), correctly set ble ROUTE id
- try to get ble working..
- temp uart ble bridge on stm
- lot of ble debugging
- nrf firmware now working
- add Watchdog, try getting ble fast (without success)
- BLE: try zello service UUID
- ble: ochange zello UUID
- Split ble telemetry
- fix ble combined binary creation
- ble: correct zello service UUID
- add nrf sw reset
- ble update receive working
- nrf: add getVersion
- nrf: add terminator
- fix: save version to config.txt file
- nrf: bootloader fw update
- few more ble update stream trial
- Bootloader: button hold >1s skips update.
- add delay to nrf ble update
- nrf update, first chunk only
- nrf update, first chunk only
- almost working
- almost working
- litte steps
- litte steps
- more
- more
- NRF updates working!
- NRF updates working!
- add igc log sd flash intervall to 5000ms
- better error log
- watchdog keepalive in bt save and getall cmd
- new prios, add rst markers
- more trials, but no sucess
- add gps mock
- wire igc logger to global flightsatus tracker
- fix multi tone output
- improve logging
- fix error message igc logging
- remove error logging in igc logger
- add config parameter "logOnlyWhenFlying"
- try to find the reset bug, lot of debug msg
- disable gps dummy
- fix tests
- add error source output to Bootloader
- BLE version 1.3.0
- BLE version 1.3.0
- fix auto shutdown logic
- bug: backwards compatibility for igc parameters for peepvario
- fix production test fw
- IGC logger real 1Hz schedule & more robust
- add audio state: OFF to double press cycle & tests
- BLE: only start ble after main uc enables, with timeout of 5s
- BLE: only start ble after main uc enables, with timeout of 5s
- ci: add nRF52805 BLE firmware build job (beta only)
- fix(nrf-ble): resolve case-sensitive version.hpp filename mismatch for Linux CI
- fix(nrf-ble): resolve case-sensitive version.hpp filename mismatch for Linux CI
- fix(nrf-ble): update version.hpp comment for lowercase filename
- fix(nrf-ble): update version.hpp comment for lowercase filename
- ci: isolate peepVario/LiftAir publish steps so one product's failure doesn't block the other
- test(nrf-ble): add host GoogleTest framework for pure-logic firmware components
- test(nrf-ble): add host GoogleTest framework for pure-logic firmware components
- ci: run nRF host unit tests after the firmware build instead of before
- ci: split nRF host tests into their own job; fix STM32 upload step that got nested inside build_nrf_firmware
- ble version read
- more delay to ble version read
- add gpsfix to XCTOD protocol
- reduce ble telemetry to 250ms
- add config command GET_GPS_STATUS
- new igc list command (20 listings)
- add utc time to gps poll
- delay ble init 3 seconds
- add 3D view via ble
- gps status: snr per satellite
- commit rest of ble bugfixes
- better gps height parsing
- short delay in nrf update
- nrf build job - app only - combined image
- temp fix ble save tonecurve
- fix gps height not sending
- igc preview
- battery percent log
- BLE: change default route to 0xFFE0
- BLE: change default route to 0xFFE0
- BL: add delay before sync byte
- bluetooth task cosmetic
- blink bootloader while trying to sync
- blink bootloader while trying to sync
- BLE: add WDG
- BLE: add WDG
- fix battery percent log
- fix error log battery write; more time for ble init 5sec
- LIFTAIR_ZERO_V3: ADD Display
- add display tests
- change display driver
- add mag correction
- add nrf workspace
- add nrf workspace
- fix ble init issues
- Initialize Bluetooth subtree history
- Merge febb733 into Bluetooth subtree
- LZ2: V120, nrf update working
- move bluetooth stuff to separate submodule

### v1.5.4:
- fix: PV ble init (from beta version)

### v1.5.5:
- Migrate user data
- Some IGC signing thoughts
- Change 3D view to Quaternion; some Orientation diagnostics
- new LZV2 version
