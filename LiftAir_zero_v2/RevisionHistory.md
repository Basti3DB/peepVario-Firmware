# Revision History
R2

# LiftAir zero v2 Firmware

### v1.0.0:
* inital version

### v1.2.0:
- move bluetooth stuff to separate submodule

### v1.2.1:
- fix: PV ble init (from beta version)

### v1.2.2:
- Migrate user data
- Some IGC signing thoughts
- Change 3D view to Quaternion; some Orientation diagnostics
- new LZV2 version

### v1.2.4:
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
