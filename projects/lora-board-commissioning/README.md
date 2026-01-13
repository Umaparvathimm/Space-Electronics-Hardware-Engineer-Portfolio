# LoRa Communication Board — Commissioning & Hardware Debugging  
**University of Würzburg | UWE-5 CubeSat Mission | 04/2023 – 09/2023**

---

## Project Overview
This project focused on the **commissioning and electrical validation** of a multi-channel **LoRa-based communication board** designed for the **University of Würzburg Experimental (UWE)-5 CubeSat mission**.  

The board was originally designed as part of a prior master’s thesis, and my role was to **bring the hardware to a testable state**, identify design or manufacturing issues, and assess readiness for mission use.

The board targets **long-range, low-power communication** using **SX1281 LoRa transceivers**, aligned with CubeSat SWaP constraints.

---

## System Architecture
- **Four independent LoRa transceiver channels**
- **Two MCUs**, each controlling two transceiver channels
- **SX1281 LoRa ICs** for long-range RF communication
- **RF front-end per channel**, including:
  - SPDT RF switch  
  - LNA with switching control  
  - RF and π-filters
- **UNISEC interface support** for CubeSat integration
- USB and UNISEC-based power options

---

## My Responsibilities
- Hardware bring-up and **board-level commissioning**
- Electrical validation against schematics and PCB layout
- Continuity, voltage, and interface testing
- Debugging manufacturing and soldering defects
- Root-cause analysis of shorts and unexpected ground connections
- Documentation of issues, mitigation paths, and future work

---

## Testing & Validation Performed

### Electrical Testing
- **Continuity testing** of power rails, MCU pins, and RF paths  
- **Voltage verification** of LDO outputs and MCU supply pins  
- Validation of USB and UNISEC power configurations  

### Debugging & Failure Analysis
- Identified **hidden shorts** between MCU pins not visible under optical inspection
- Detected multiple:
  - Pin-to-pin shorts  
  - Pin-to-ground shorts  
  - RF path grounding issues  
- Traced faults across:
  - MCU-B soldering defects  
  - Transceiver-to-MCU interface pins  
  - RF front-end components  

### Key Findings (Examples)
- MCU-B pins shorted internally and to ground (likely soldering or pad-related)
- Multiple SX1281 transceiver channels affected by shorted SPI and RF pins
- RF front-end components showing unexpected grounding
- USB-B data pins unintentionally grounded

These findings directly impacted board usability and required mitigation before software validation.

---

## Tools & Equipment Used
- **Multimeter** (continuity & voltage testing)
- Oscilloscope (basic signal validation)
- **STM32 CubeIDE** for MCU programming
- JTAG/SWD for debugging and flashing
- Hardware schematics & PCB layout review

---

## Engineering Skills Demonstrated
- Board bring-up under non-ideal conditions
- Systematic hardware debugging methodology
- Reading schematics and correlating them to physical layout
- Identifying manufacturing vs. design-induced failures
- Understanding RF signal paths and sensitivity to grounding
- Clear documentation of hardware issues and next steps

---

## Outcome
- Board was **not mission-ready** in its received state
- Root causes of failures were identified and documented
- Clear mitigation and rework steps were proposed
- Provided a solid basis for future redesign or reassembly

This project reinforced the importance of **DFT-aware design**, manufacturability checks, and thorough electrical validation before software integration.

---

## What This Project Shows
- Hands-on experience with **real, imperfect hardware**
- Ability to debug complex mixed-signal and RF boards
- Comfort working close to hardware during early bring-up
- Strong attention to detail and engineering judgment
- Willingness to document failures honestly — critical for space hardware

---

### 📌 Note on Documentation
Detailed schematics and full design files are not shared publicly due to academic and project constraints.  
The content here focuses on **engineering process, testing methodology, and lessons learned**.
