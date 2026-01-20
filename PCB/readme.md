🩸 OpenSpO₂ – Custom Pulse Oximeter Hardware
Overview

OpenSpO₂ is a custom-designed pulse oximeter hardware system for measuring blood oxygen saturation (SpO₂) and heart rate using optical pulse oximetry.
The design is split into two schematics: a sensor power & interface module and a discrete analog signal conditioning + ADC module.

This project is intended for educational, prototyping, and research purposes.

📐 Schematics Structure
1️⃣ Schematic 1 – Sensor Power & Digital Interface

📄 SCH_Schematic1_2026-01-20.pdf 

SCH_Schematic1_2026-01-20

This schematic focuses on power regulation and digital communication for the SpO₂ sensor module.

Key Functions:

Accepts 5V input power

Generates regulated 3.3V and 1.8V rails

Interfaces with the MAX30102 optical SpO₂ sensor

Provides I²C (SCL, SDA) output for external controllers

Major Blocks:

LP2985 LDO regulators for low-noise voltage regulation

MAX30102 integrated SpO₂ sensor (Red + IR LEDs, photodiode)

I²C pull-up resistors

Input/output pin headers for power and data

This schematic can be used as a standalone SpO₂ sensor module.

2️⃣ Schematic 2 – Analog Front-End & ADC Processing

📄 SCH_Schematic3_2026-01-20.pdf 

SCH_Schematic3_2026-01-20

This schematic implements a fully discrete pulse oximetry analog front-end, suitable for learning and experimentation.

Key Functions:

Drives Red (660 nm) and IR (940 nm) LEDs

Captures reflected/transmitted light using a photodiode

Amplifies and filters the PPG signal

Converts analog signals to digital using a high-resolution ADC

Major Blocks:

BC847B transistor drivers for LED PWM control

BPW34 photodiode for optical sensing

OPA333 precision op-amp for low-noise amplification

TL081 op-amp for additional signal conditioning

ADS1115 (16-bit ADC) with I²C interface

RC networks for filtering and biasing

This schematic demonstrates the core electronics behind pulse oximetry, without relying on a fully integrated sensor IC.

🔗 System Architecture
[ Finger / Tissue ]
        ↓
[ Red & IR LEDs ]
        ↓
[ Photodiode ]
        ↓
[ Analog Amplification & Filtering ]
        ↓
[ ADS1115 – 16-bit ADC ]
        ↓
[ I²C Interface ]
        ↓
[ Microcontroller / SBC ]
