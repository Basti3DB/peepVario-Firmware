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
