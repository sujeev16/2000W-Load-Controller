# 2000W-Load-Controller
2000W EV Load Controller for  Gray Mobility 
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
