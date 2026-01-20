This project uses discrete optical, analog, and digital components to implement a custom SpO₂ sensor. The design includes regulated power management, dual-wavelength LEDs for optical sensing, low-noise amplification, high-resolution ADC data acquisition, and passive components for signal conditioning, filtering, and stability.


| No. | Quantity | Designator(s) | Component | Value / Part No. | Footprint | Category |
|----|----------|--------------|-----------|------------------|-----------|----------|
| 1 | 1 | C1 | Capacitor | 10 µF | 0603 | MLCC |
| 2 | 6 | C3, C4, C6, C8, C10, C11 | Capacitor | 0.1 µF | 0603 | MLCC |
| 3 | 1 | C5 | Capacitor | 15 nF | 0603 | MLCC |
| 4 | 1 | C7 | Capacitor | 10 nF | 0603 | MLCC |
| 5 | 1 | C9 | Capacitor | 1 µF | 0603 | MLCC |
| 6 | 4 | C12, C13, C14, C15 | Capacitor | 100 nF | 0603 | MLCC |
| 7 | 3 | GND, VCC, PWM | Pin Header | 2-Pin (2.54 mm) | Through-Hole | Connector |
| 8 | 1 | IR | Infrared LED | VSMB3940X01-GS08 | SMD | Optoelectronics |
| 9 | 2 | irpwm, redpwm | NPN Transistor | BC847B | SOT-23 | BJT |
|10 | 1 | Photodec | Photodiode | BPW34 | Through-Hole | Sensor |
|11 | 2 | R1, R2 | Resistor | 150 Ω | 0603 | Passive |
|12 | 1 | R3 | Resistor | 1 MΩ | 0603 | Passive |
|13 | 1 | R4 | Resistor | 3.18 MΩ | 0603 | Passive |
|14 | 1 | R5 | Resistor | 31.8 MΩ | 0603 | Passive |
|15 | 2 | R6, R7 | Resistor | 4.7 kΩ | 0603 | Passive |
|16 | 3 | R8, R9, R10 | Resistor | 10 kΩ | 0603 | Passive |
|17 | 1 | Red | Red LED | SFH4059 | SMD | Optoelectronics |
|18 | 1 | U2 | ADC | ADS1115 | VSSOP-10 | IC |
|19 | 1 | U3 | Op-Amp | OPA333 | SOIC-8 | IC |
|20 | 1 | U4 | Op-Amp | TL081 | SOP-8 | IC |
|21 | 1 | vltreg-5v | LDO Regulator | LP2985-50 | SOT-23-5 | Power |


- All passive components use 0603 SMD packages.
- Dual-wavelength LEDs (Red + IR) are used for SpO₂ measurement.
- ADS1115 provides high-resolution ADC for photodiode signal acquisition.
- OPA333 and TL081 are used for low-noise analog signal conditioning.







