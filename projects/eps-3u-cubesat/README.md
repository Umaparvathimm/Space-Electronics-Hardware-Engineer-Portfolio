# Next-Generation Electrical Power System (EPS) for 3U CubeSat  
**Zentrum für Telematik (ZfT), Würzburg** · **10/2023 – 03/2024**

---

## Overview
This project involved the **design, implementation, assembly, and testing of a next-generation Electrical Power System (EPS)** for a 3U CubeSat platform. The EPS was designed to support 8 battery packs, provide regulated power distribution, and enable reliable monitoring and control.

---

## System Architecture

### Electrical Power System (EPS) Board
![EPS Board Block Diagram](images/EPS1.png)

### Battery Board
![Battery Board Block Diagram](images/EPS2.png)

---

## What I Worked On
- End-to-end development of a **flight-like EPS board** supporting **8 battery packs**
- Definition of EPS architecture including power generation, regulation, and distribution
- **MCU-based control and monitoring** of battery packs and power paths
- Designing of power path protection circuitry
- Component selection with attention to reliability and space-system constraints
- Close coordination with system-level requirements and CubeSat interfaces

---

## Schematic & PCB Development
- Schematic capture and **6-layer PCB design** using **KiCad**
- Careful separation of power and control domains
- Design decisions guided by **Design for Manufacturability (DFM)** and **Design for Testability (DFT)** principles:
  - Test-point accessibility for key power rails
  - Clear partitioning of functional blocks
  - Layout choices supporting bring-up and debugging

---

## Simulation
- Circuit-level simulations using **LTSpice**
- Validation of:
  - Power regulation behavior
  - Load response and stability
  - Voltage and current sensing circuitry
  - Battery regulation concepts
- Simulation results used to guide design refinement prior to fabrication

---

## Assembly & Bring-Up
- Assembly of the EPS PCB and supporting hardware using a pick and place machine
- Step-by-step board bring-up:
  - Verification of power rails
  - Controlled activation of subsystems
  - Incremental validation of functionality
- Identification and resolution of hardware issues during early testing

---

## Testing & Validation
- **Power-path validation** under representative operating conditions
- Battery regulation and charging behavior testing
- Efficiency measurements and load testing
- Hardware debugging using:
  - Oscilloscopes
  - Multimeters
  - Power analysis tools

---

## Tools & Skills Demonstrated
- **Power electronics:** battery management, regulation, and distribution
- **PCB design:** KiCad (6-layer board)
- **Simulation:** LTSpice
- **Testing:** oscilloscope, multimeter, power analysis tools
- **Embedded control:** MCU-based monitoring and control concepts
- **System integration:** EPS interaction with other CubeSat subsystems

---

## What This Project Shows
- Ability to design and bring up complex power electronics for space systems
- Hands-on experience with PCB assembly, debugging, and validation
- Practical understanding of power subsystem reliability and testing
- Confidence working close to real hardware in a mission-oriented environment
