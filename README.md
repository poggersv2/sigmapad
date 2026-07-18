# Sigmapad

Sigmapad is a 9-key macropad in a 3x3 grid with an EC11 rotary encoder. It runs on QMK firmware. 

It was built as part of Hack Club's Stardance and Hackpad programs to handle frequently used shortcuts.

## Features
- 9 Keys in a standard 3x3 grid.
- EC11 Rotary encoder (with built-in push switch) for whatever you want.
- USB-C connectivity.

## CAD Model
The case consists of three printed parts: the top frame, the switch plate, and the bottom enclosure. 
Everything fits together using four M3x16mm screws and M3 heat-set inserts.

<img src="https://github.com/poggersv2/sigmapad/blob/main/assets/readme/case-front.png" alt="Case Front" height="300"/>
<img src="https://github.com/poggersv2/sigmapad/blob/main/assets/readme/case-exploded.png" alt="Case Exploded" height="300"/>

## PCB
Here's the schematic and board layout. 

<img src="https://github.com/poggersv2/sigmapad/blob/main/assets/readme/schematic.png" alt="Schematic" height="300"/>
<img src="https://github.com/poggersv2/sigmapad/blob/main/assets/readme/pcb-front.png" alt="PCB Front" height="300"/>
<img src="https://github.com/poggersv2/sigmapad/blob/main/assets/readme/pcb-back.png" alt="PCB Back" height="300"/>
<img src="https://github.com/poggersv2/sigmapad/blob/main/assets/readme/pcb.png" alt="PCB" height="300"/>

## Firmware Overview
## Firmware Overview
This macropad uses [QMK](https://qmk.fm/) firmware. 
The rotary encoder changes volume and mutes on press. 
The default keys are:

```text
┌───┬───┬───┐
│ Q │ W │ E │
├───┼───┼───┤
│ A │ S │ D │
├───┼───┼───┤
│ Z │ X │ C │
└───┴───┴───┘
```

To flash the board, compile your `.uf2` file, hold the BOOT button on the RP2040 while plugging it in, and drag the file onto the mounted drive. 

## BOM
Here is everything you need to build this macropad:

- 1x Seeed Studio XIAO RP2040
- 9x Cherry MX-style Switches
- 9x White Blank DSA Keycaps
- 9x Through-hole 1N4148 Diodes
- 1x EC11 Rotary Encoder
- 4x M3x16mm Screws
- 4x M3x5x4mm Heat-set Inserts
- 1x Case (Top, Plate, Bottom)

## Extra stuff
**Tools I used:**
* **CAD:** Fusion
* **PCB and Schematic:** KiCad
