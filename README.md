# STRF
PCB Designing 

## Overview

This repository contains the complete hardware design of my **4-layer USB Type-C enabled RF development board**, designed using **KiCad**. The project was developed to gain hands-on experience in professional PCB design, RF hardware design, and embedded systems.

The board combines an **STM32L4 microcontroller**, **Semtech SX1272 LoRa transceiver**, **USB Type-C interface**, and **MicroSD card support** into a compact multilayer PCB suitable for long-range wireless communication applications.

From schematic capture to PCB layout, design verification, and Gerber generation, this project follows a complete hardware development workflow similar to what is used in the electronics industry.

---
The objective of this project was to understand the complete PCB design process while learning industry-standard design practices.
# Board Features

- 4-Layer PCB Design
- STM32L4 Low-Power Microcontroller
- Semtech SX1272 LoRa RF Transceiver
- USB Type-C Interface
- MicroSD Card Interface
- SWD Programming Header
- RF Matching Network
- 50 Ω RF Output
- Power Distribution Network
- Reset Circuit
- Status LEDs
- Decoupling Capacitors
- Ground Stitching Vias
- Manufacturing-Ready Gerber Files

---

## Board Specifications

- **Board Size:** 31 mm × 70 mm

# PCB Stack up
Layer-1-- signal
Layer-2-- Ground
Layer-3-- 3v3 
Layer-4-- signal 



### Power Stage

The board is powered through a USB Type-C connector.

The onboard voltage regulation circuit converts the input voltage into a stable 3.3 V supply required by the STM32L4 microcontroller and the SX1272 RF transceiver.

---

### Processing Unit

The STM32L4 acts as the brain of the system.

It is responsible for:

- Running application firmware
- Controlling onboard peripherals
- Communicating with the LoRa transceiver
- Reading external sensors
- Managing data storage
- Processing received wireless packets

---

### LoRa Communication

The SX1272 communicates with the STM32 over the SPI interface.

When the microcontroller needs to transmit data:

 The STM32 sends data through SPI.The SX1272 converts the data into a LoRa RF signal. The RF matching network optimizes the signal. The antenna transmits the wireless packet.

Similarly, received RF packets are demodulated by the SX1272 and transferred back to the STM32 for processing.

---

### Data Storage

The onboard MicroSD card interface allows external storage of sensor readings, logs, or application data.

Communication with the MicroSD card is performed using SPI. 

# Project Workflow

This project was completed following the standard PCB development process.

- Requirement Analysis
- Component Selection
- Schematic Design
- Symbol Verification
- Footprint Assignment
- PCB Floor Planning
- Component Placement
- Routing
- Ground Plane Design
- RF Layout Optimization
- USB Differential Pair Routing
- Design Rule Check (DRC)
- Electrical Rule Check (ERC)
- Gerber Generation
- Manufacturing File Preparation

# Project Workflow

This project was completed following the standard PCB development process.

- Requirement Analysis
- Component Selection
- Schematic Design
- Symbol Verification
- Footprint Assignment
- PCB Floor Planning
- Component Placement
- Routing
- Ground Plane Design
- RF Layout Optimization
- USB Differential Pair Routing
- Design Rule Check (DRC)
- Electrical Rule Check (ERC)
- Gerber Generation
- Manufacturing File Preparation

# Tools Used

- KiCad
- STM32L4 Reference Manual & Datasheet
- Semtech SX1272 Datasheet
- JLCPCB Design Guidelines


# schematic 
<img width="1167" height="821" alt="Screenshot 2026-08-14 23073" src="https://github.com/user-attachments/assets/677fc8c3-8f8a-4137-999c-713ecb0ee3cf" />

# PCB Layout
<img width="1432" height="711" alt="Screenshot 2026-08-14 230947" src="https://github.com/user-attachments/assets/7438807a-1d20-499d-9b97-64694f47cc87" />

# 3D View
<img width="1675" height="892" alt="device_top_view" src="https://github.com/user-attachments/assets/003c7fa1-fa25-46fb-bf4b-24ce08492021" />

<img width="1675" height="892" alt="device_bottom_view" src="https://github.com/user-attachments/assets/cbafc0ed-d89b-4172-826e-3d99471727d1" />





















# About Me

**Ganesh Naik**

Electronics and Communication Engineering Student












