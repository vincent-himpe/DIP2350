# DIP2350
## An RP2350 Packaged as a 64 pin DIP package that fits a standard 64pin dip socket (motorola MC68000 style)

### Overview

- USB Type-C connector. Right angle , thru hole for mechanical stability. long overhang so you can have this go through an enclosure wall
- USB powered or self powered. self powered up to 12 volt
- ideal diode / or-ing / e-fuse circuit (optional) to prevent backfeeding usb. Current limit on the ideal diode. the circuit can be used as a power or-ing to provide backup power from a Li-Ion cell and charger
- ESD protection on the USB port using TVS diodes
- 3v3 DC/Dc regulator can deliver up to 1A of load current. In this case you need to provide 5v as USB cannot provide source current.
- RP2350B in 80 pin QFN with all 48 GPIO brought out.
- Flash 128Mbit
- optional PSRAM on GPIO47
- optional 3v reference for analog circuitry LM4040-3
- Heartbeat led on gp25 with solder bridge. Can be removed from circuit.
- using abracon XTAL and polarized inductor for 1v1 regulator
- boot and reset button. secondary boot button under usb so you can use a paperclip through the enclosure to force boot.
- on board, optional i2c bus :
- - I2C EEPROM or FRAM
  - I2C RTC with battery backup 1220 cell.
  - - cheap version using an M41t11
    - precision using a MEMS DS3231. option to use brown-out detection to hold cpu in reset till power stabilizes. optional interrupt on GPIO21. User needs to wire the i2c bus to desired io port.
- 4 layer board with controlled impedance and power planes. Board designed so it can be made at OshPark, JLCPCB or PCBway
- CAD source available under Creative Commons ZERO . Public Domain License. Altium Format. 
- Production pack (gerber/drill/bom available.
- BOM is procurable from Digikey/Mouser as well as LCSC (Asia) with direct LCSC order codes if you want his to be partially assembled by JLCPCB.
  

![DIP2350 FRONT](https://github.com/user-attachments/assets/cd2cd542-4e73-4b8e-a0bb-81699b13926e)

![DIP2350 BACK](https://github.com/user-attachments/assets/3e79bf61-8e5a-404c-a834-e33eb9c5390c)


## Schematic

[DIP2350 SCHEMATIC - RC0.pdf](https://github.com/user-attachments/files/20359181/DIP2350.SCHEMATIC.-.RC0.pdf)

