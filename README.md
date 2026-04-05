# 2000W Load Controller — Gray Mobility 

![KiCad](https://img.shields.io/badge/KiCad-8.0-blue)
![LTspice](https://img.shields.io/badge/LTspice-XVII-orange)
![Status](https://img.shields.io/badge/Status-Complete-green)
![PCB](https://img.shields.io/badge/PCB-2Layer_FR4-yellow)

## Overview
Complete hardware design for a 2000W DC load controller 
for electric vehicle applications. Accepts 40V DC input 
and drives a 36V/56A LED load using MOSFET switching 
topology controlled by STM32 microcontroller.

## System Specifications
| Parameter | Value |
|-----------|-------|
| Input Voltage | 40V DC |
| Output Voltage | 36V DC |
| Continuous Current | 56A |
| Peak Current | 100A |
| Switching Frequency | 10kHz |
| MCU | STM32F103C4Tx |
| Temperature Sensors | 4x NTC 10K |
| PCB | 2-layer FR4 2oz copper |

## Repository Structure
2000W-Load-Controller/
├── Block_Diagram/
│   └── Block_Diagram.pdf
├── Schematic/
│   └── Schematic.pdf
├── PCB/
│   └── PCB_Layout.pdf
├── Gerbers/
│   └── All .gbr files
├── Simulation/
│   └── LTspice files + waveforms
└── Documentation/
├── BOM_and_Writeup.docx
└── BOM.csv
## Features
- LM2596S buck converter 40V → 36V
- IRF540N MOSFET switching at 10kHz
- ULN2003 gate driver
- STM32F103 32-bit microcontroller
- 4x NTC temperature sensing
- OVP on all rails via Zener diodes
- OCP via 0.01Ω shunt resistor
- 100A blade fuse protection
- LM1117 3.3V MCU supply

## Tools Used
| Tool | Purpose |
|------|---------|
| KiCad 8 | Schematic + PCB design |
| LTspice XVII | Circuit simulation |
| draw.io | System block diagram |

## Simulation Results
MOSFET gate drive circuit verified in LTspice:
- Gate: Clean 0V ↔ 5V at 10kHz ✅
- Drain: Switching 36V ↔ 0V ✅  
- Load current: ~56A pulses ✅

## Note
Physical hardware assembly not completed due to component 
unavailability. All design deliverables complete and 
simulation verified.

## Author
**Sujeev Ravindra Swami**  
B.E. Electronics and Communication Engineering  
JSS Academy of Technical Education, Bangalore (2025)
