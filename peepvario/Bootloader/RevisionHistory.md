# Revision History

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

###  	v1.2.0:
* add recovery firmware update via BLE

###  	v1.2.1:
* fix valid firmware detection

###  	v1.2.2:
* lower min FW size
* higher max FW size

###  	v1.3.0:
* change usb volume name

###  	v1.4.0:
* better audio quality

### v1.4.3:
- Add UTC start time to Bluetooth IGC preview
- add Thermal assistant for LZV2 & 3
- build before launch
- LZV2 HW changes
- reduce error piep duration from 10 to 5 sec
- Update automatic github workflow to only build needed submodules
- fix igc flight log sorting
- Rise HAL_GET_TICK prio to 3, to fix hangers
- first step for gps receiver maxm10
- ble filesystem nav command
- Bootloader double peep
- remove nrf update fw after update
- auto detect corrupted files on sdcard
- add GPS soft disable/enable
- fix config read on sdcard after fw update
- fix data migration on eeprom after updates
- fix stackoverflow when using ble config website
- no 15min autoshutdown when usb is connected
- Refactor: Move tasks to Helpers directory
- fix lzv2 production test
- lzv3 display kinda working
- lzv3 display integrated
- improove thermal assistant
- fix audio volume change beep delay
- fix fake buttonpress after statup while usb connected
- add LZV3 display animations
- faster ble disconnect detection
- rename Filesystem volume name
- apply filesysteme volume name to all products
- add heartbeat blinks to bootloader
- auto delete old IGCs when full
- automatic nrf fw recovery
- add nrf ble bootloader updater
- add ble bootloader query
- github auto push for bootloaders (main)
- peepVario Bootloader size improovement
