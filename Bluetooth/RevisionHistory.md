# Revision History
R1

# Bluetooth Firmware

### v1.0.0:
* initial version

### v1.1.0:
* reports version 1.0.0
* add ble update command

### v1.2.0:
* reports version 1.0.0
* add experimental Zello ble service

### v1.3.0:
* update-able
* separate bootloader

### v1.4.0:
* fix boot race condidtion when ble is connected

### v1.4.1:
* App update only (no Softdevice)

### v1.4.3:
* fix boot init error

### v1.4.4:
* fix ble update

### v1.4.5:
* Production App-only BIN: LiftAir_BLE_App_v145.bin
* Source: https://github.com/Basti3DB/peepVario-dev-NRF/commit/77ca87c554e138376edf12d7db0a6f8a1a993050
* Build and host tests: https://github.com/Basti3DB/peepVario-dev-NRF/actions/runs/42373913820

### v1.5.1:
* Production App-only BIN: LiftAir_BLE_App_v151.bin
* Source: https://github.com/Basti3DB/peepVario-dev-NRF/commit/4e87e1259a3cfb322ed4db4d3733782c94279c8a
* Build and host tests: https://github.com/Basti3DB/peepVario-dev-NRF/actions/runs/42606599974

### Bootloader v0.3.0:
* Production bootloader update BIN (stream via app command 0x27): Bootloader/LiftAir_BLE_Bootloader_v030.bin
* Source: https://github.com/Basti3DB/peepVario-dev-NRF/commit/4e87e1259a3cfb322ed4db4d3733782c94279c8a
* Build and host tests: https://github.com/Basti3DB/peepVario-dev-NRF/actions/runs/42606599974
