# LiftAir zero v2 beta Firmware

### v1.0.0 _ 1:
* 


### v1.0.0 _ 1:
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

### v1.0.0 _ 2:
- remove unwanted default ble telemetry data
- Change hardcoded MagnetSensor orientation "flip"
- move BootloaderUpdater into LiftAirzeroV2 product (instead of separate FW needed)
- lower preamble pusle (nicer audio)
- Tune ESKF
- add experimental touch detection

### v1.0.0 _ 3:
- change the touch detection to double-press

### v1.0.0 _ 4:
- add a touch delay for double press

### v1.1.0 _ 1:
- fix crash at gps fix
- write correct IGC header

### v1.1.0 _ 2:
- fix crash at gps fix #2
- fix sensortask&audiotask crash


### v1.1.0 _ 3:
- fix production test fw

### v1.1.0 _ 4:
- IGC logger real 1Hz schedule & more robust
- add audio state: OFF to double press cycle & tests
- BLE: only start ble after main uc enables, with timeout of 5s

### v1.1.0 _ 5:
- ble version read

### v1.1.0 _ 6:
- more delay to ble version read
- add gpsfix to XCTOD protocol
- reduce ble telemetry to 250ms
- add config command GET_GPS_STATUS
- new igc list command (20 listings)

### v1.1.0 _ 7:
- commit rest of ble bugfixes

### v1.1.0 _ 8:
- better gps height parsing
- short delay in nrf update
- nrf build job - app only - combined image
- temp fix ble save tonecurve

### v1.1.0 _ 9:
- fix gps height not sending

### v1.1.0 _ 10:
- igc preview

### v1.1.0 _ 11:
- battery percent log
- BLE: change default route to 0xFFE0
- BL: add delay before sync byte
- bluetooth task cosmetic
- blink bootloader while trying to sync
- BLE: add WDG
- fix battery percent log
- fix error log battery write; more time for ble init 5sec
- LIFTAIR_ZERO_V3: ADD Display
- add display tests

### v1.1.0 _ 12:
- change display driver
- add mag correction

### v1.2.0 _ 1:
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
- nrf update, first chunk only
- almost working
- litte steps
- more
- NRF updates working!
- BLE version 1.3.0
- BLE: only start ble after main uc enables, with timeout of 5s
- fix(nrf-ble): resolve case-sensitive version.hpp filename mismatch for Linux CI
- fix(nrf-ble): update version.hpp comment for lowercase filename
- test(nrf-ble): add host GoogleTest framework for pure-logic firmware components
- BLE: change default route to 0xFFE0
- blink bootloader while trying to sync
- BLE: add WDG
- add nrf workspace
- add nrf workspace
- fix ble init issues
- Initialize Bluetooth subtree history
- Merge febb733 into Bluetooth subtree
- LZ2: V120, nrf update working
- move bluetooth stuff to separate submodule

### v1.2.0 _ 2:
- remove nrf from auto deploy
- verify nrf version read
- fix: nrf version read final
