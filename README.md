# 🧪 Two-Stage Operational Transconductance Amplifier (OTA) – GPDK180

This repository contains the design, simulation, and analysis of a **Two-Stage OTA** using **Cadence Virtuoso** and **GPDK180 (180 nm CMOS)**. The project includes the schematic design, AC response simulation, and performance analysis based on standard analog design specifications.

---

## 🔧 Design Specifications

- **Technology**: 180 nm (GPDK180)
- **Process Constants**:
  - \( K'_n = 300\ \mu A/V^2 \)
  - \( K'_p = 75\ \mu A/V^2 \)
  - \( V_{TN} = -V_{TP} = 0.5\ V\) or \(0.35\ V\)
- **DC Gain** ≥ 60 dB  
- **Gain Bandwidth Product (GBW)** ≥ 30 MHz  
- **Phase Margin (PM)** ≥ 60°  
- **Slew Rate** ≥ 20 V/μs  
- **Load Capacitance (CL)** = 2 pF  
- **Power Dissipation** ≤ 300 μW  
- **Input Common Mode Range (ICMR)**: 0.8 V – 1.6 V  
- **Supply Voltage**: ±1.8 V  
- **Compensation Capacitance (Cc)** = 800 fF  
- **Bias Current (Is)** = 20 μA

---

## ⚙️ Transistor Sizing

| Transistor | Width (W) | Length (L) |
|------------|------------|-------------|
| M1, M2     | 3 μm       | 500 nm      |
| M3, M4     | 7 μm       | 500 nm      |
| M5, M8     | 6 μm       | 500 nm      |
| M6         | 87 μm      | 500 nm      |
| M7         | 37.5 μm    | 500 nm      |

---

## 🖼️ Circuit Schematic

Below is the two-stage OTA architecture used in this design:

![Two-Stage OTA Schematic](./3e3c2199-68a8-45f2-a45b-f923b0641105.png)

---

## 📈 Simulation Result

### ➤ AC Response (Gain & Phase)

- Shows the frequency response with gain ≥ 60 dB and phase margin ≥ 60°

![AC Response](results/ac_response_gain_phase.png)


---

## 🛠️ Tools Used

- Cadence Virtuoso (ADE L, Visualization & Analysis XL)
- Spectre Simulator
- GPDK180 Technology Library

---

## 📌 Notes

This is an academic project intended for learning analog CMOS design. You are free to fork or contribute for layout extension, Monte Carlo simulation, or further noise analysis.


