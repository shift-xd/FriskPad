# FriskPad
FriskPad is Hackpad version iteration by frisky lmao
 
## Hackpad Overview

<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/0bb2b030-12ee-47bb-9e50-c46efde315f4" />


This shows the full assembly of FriskPad in Fusion 360.  
It demonstrates how the PCB, case, and components fit together.

## Features

- Seeed XIAO RP2040 microcontroller  
- 0.91" I2C OLED display  
- 3x3 mechanical key layout 
- Direct wiring for every key 


## Schematic
<img width="583" height="318" alt="image" src="https://github.com/user-attachments/assets/785be22d-1afe-44d3-bf2b-3f90afd3a17f" />



The schematic was designed in KiCad.  
Each switch connects directly to the RP2040.  
The OLED follows GND, VCC, SCL, SDA pin order.

## PCB Layout
<img width="246" height="318" alt="FriskPad PCB" src="https://github.com/user-attachments/assets/bfbd05e2-5d72-47e0-8b58-85c296c94221" />

The PCB was designed in KiCad PCB Editor.  
It shows component placement and routing.  
The layout focuses on clarity and simplicity.




## Case Design
<img width="573" height="325" alt="FriskPadCase Only Image " src="https://github.com/user-attachments/assets/fac86dd9-5b5a-41de-9908-b06017ad07ac" />
<img width="573" height="325" alt="FriskPad Case With PCB render " src="https://github.com/user-attachments/assets/abbc7b61-9597-42f5-8c72-65ff03f5cca8" />

### Nothing much just wanted to add i hate screws the lid is a snap fit mechanism which i will glue together with removable fevibond gum i have 

The case was designed in Free Cad .  
Dimensions were taken directly from the PCB.  
All parts were test-fit using 3D models.

## Bill of Materials

| Part | Quantity | Description |
|------|----------|-------------|
| Mechanical key switches | 9 | MX-style |
| Keycaps | 9 | MX-compatible |
| Seeed XIAO RP2040 | 1 | Microcontroller |
| OLED display (0.91") | 1 | I2C |
| PCB | 1 | Double-sided |
| Case | 1 | 3D printed |

## Firmware Instructions

### Flashing

1. Install CircuitPython `.uf2`.
2. Enter bootloader mode.
3. Copy the `.uf2` to the board.

### Libraries

1. Download CircuitPython library bundle.
2. Copy `displayio`, `display_text`, `debouncer`, and `HID`.
3. Upload `code.py`.
4. Test all inputs.

## License

This project is open source under the MIT License.
