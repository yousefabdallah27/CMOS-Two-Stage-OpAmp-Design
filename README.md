# CMOS Two-Stage Operational Amplifier Design (130nm)

## 📌 Project Overview
This repository details the complete design flow, hand analysis, and Cadence Virtuoso simulation results for a Two-Stage CMOS Operational Amplifier. The design was implemented using a **0.13-µm (130nm) CMOS process**. 

The objective of this project was to design a stable and highly efficient Op-Amp utilizing Miller compensation to guarantee loop stability, meeting specific target parameters including a high Unity Gain Frequency (GBW) and a specific Output DC-level.

## 📊 Design Specifications (Target vs. Achieved)
The following table compares the target design constraints against the achieved post-simulation results:

| Parameter | Target Specification | Achieved Result |
| :--- | :--- | :--- |
| **Technology Node** | 0.13-µm CMOS | 0.13-µm CMOS |
| **Supply Voltage (VDD)** | 1.2 V | 1.2 V |
| **Load Capacitance (CL)**| 0.2 pF | 0.2 pF |
| **Input DC Level** | 0.7 V | 0.7 V |
| **Output DC-Level** | 0.7 ± 0.1 V | ~593.8 mV |
| **DC Gain** | ≥ 80 dB | 57 dB |
| **Unity Gain Freq (GBW)**| ≥ 600 MHz | 600 MHz |
| **Phase Margin** | ≥ 50° | 51° |
| **Slew Rate** | ≥ 9 V/µs | Extracted from transient (ΔV/Δt) |
| **Power Consumption** | ≤ 2 mW | Verified via simulation |

## 📂 Repository Structure
- `Docs/`: Contains the project presentation, problem statement, and detailed reports.
- `Schematics/`: Screenshots of the basic Op-Amp structure and testbenches from Cadence Virtuoso.
- `Calculations/`: Hand analysis and small-signal model calculations.
- `Simulations/`: Simulation plots including Power Consumption, Phase margin, DC gain, Output DC-level, and Slew Rate transient response.

## 🛠️ Tools & Technologies
- **EDA Tool:** Cadence Virtuoso
- **Analysis:** AC, DC, and Transient Analysis
- **Compensation:** Miller Compensation
