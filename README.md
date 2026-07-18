# Sigmapad

A macropad for frequently used shortcuts, built as part of Hack Club's Stardance and Hackpad programs.

## Features

* **Minimalist design:** Clean, compact, and keeps your desk free of clutter.
* **Standard grid:** 9 keys in a 3x3 layout.
* **Rotary encoder:** EC11 encoder with a built-in push switch for custom bindings.
* **Connectivity:** USB-C.

## Hardware Design

![Case Screenshot](https://github.com/poggersv2/sigmapad/blob/main/assets/readme/case-front.png)

### Schematic
![Schematic Screenshot](https://github.com/poggersv2/sigmapad/blob/main/assets/readme/schematic.png)

### PCB Layout
![PCB Front Screenshot](https://github.com/poggersv2/sigmapad/blob/main/assets/readme/pcb-front.png)
![PCB Back Screenshot](https://github.com/poggersv2/sigmapad/blob/main/assets/readme/pcb-back.png)
![PCB Screenshot](https://github.com/poggersv2/sigmapad/blob/main/assets/readme/pcb.png)

### Case & Assembly
The case consists of three main parts: the top frame, the switch plate, and the bottom enclosure.

![Case Assembly Screenshot](https://github.com/poggersv2/sigmapad/blob/main/assets/readme/case-exploded.png)

## Bill of Materials (BOM)

| Qty | Part Description |
| :---: | :--- |
| 1 | Seeed Studio XIAO RP2040 |
| 9 | Through-hole 1N4148 Diodes |
| 9 | Cherry MX-style Switches |
| 1 | EC11 Rotary Encoder |
| 9 | White Blank DSA Keycaps |
| 4 | M3x16mm Screws |
| 4 | M3x5mmx4mm Heat-set Inserts |

## Firmware

This macropad runs on QMK. 

1. **Compile** your QMK firmware to generate a `.uf2` file for the XIAO RP2040. *(If you haven’t set up your QMK build environment yet, refer to the official QMK documentation).*
2. **Enter bootloader mode** by holding the `BOOT` button on the RP2040 while plugging it into your computer via USB.
3. **Flash the board** by dragging and dropping the compiled `.uf2` file onto the mounted drive, or by using QMK Toolbox.
4. **Reboot and test** the switches and ensure your encoder knob registers correctly.
