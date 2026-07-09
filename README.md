# Class AB Audio Power Amplifier Simulation using LTspice

## Project Overview

This project presents the design, simulation, and performance analysis of a **Class AB Audio Power Amplifier** using **LTspice**.

The amplifier combines the advantages of Class A and Class B amplifiers by providing high linearity with improved efficiency while minimizing crossover distortion. Various analyses were performed to evaluate the amplifier's performance, including transient analysis, FFT analysis, distortion analysis, and efficiency analysis.

---

## Objectives

- Design a Class AB Audio Power Amplifier.
- Simulate the amplifier in LTspice.
- Verify signal amplification through transient analysis.
- Analyze the output spectrum using FFT.
- Study distortion characteristics.
- Calculate amplifier efficiency.

---

## Software Used

- LTspice XVII

---

##  Circuit Diagram

Below is the complete LTspice schematic used for the simulation.

<p align="center">
   <img width="800" alt="image" src="https://github.com/user-attachments/assets/b089dc9f-d8e3-47e1-9855-b300359a176f" />

</p>

---

## Block Diagram

The signal flow of the amplifier is shown below.

```
Input Signal
      │
      ▼
Pre-Amplifier
      │
      ▼
Interstage Coupling & Bias Network
      │
      ▼
Class AB Output Stage
      │
      ▼
Speaker
```

---

#  Simulation Results

## 1️ Transient Analysis

The transient analysis verifies that the amplifier correctly amplifies the input signal.

### Waveforms
<p align="center">
    <img width="800" alt="image" src="https://github.com/user-attachments/assets/63d06767-478d-45d8-a55a-1acde4ff27e6" />
</p>

### Observation

- Output waveform follows the input waveform.
- Desired voltage amplification is achieved.
- Very little crossover distortion is observed.
- Output remains stable throughout the simulation.

---

## 2️ FFT Analysis

FFT analysis was performed to examine the frequency components of the output signal.


<p align="center">
    <img width="800" alt="image" src="https://github.com/user-attachments/assets/ccb94c46-2c86-4932-bba8-a421b7eb2dab" />

</p>

### Observation

- Fundamental frequency has the highest magnitude.
- Harmonic components are comparatively smaller.
- Indicates good audio signal quality.
- Low harmonic distortion is observed.

---

## 3️ Distortion Analysis

The distortion analysis evaluates the quality of the amplified signal.

<p align="center">
    <img width="800" alt="image" src="https://github.com/user-attachments/assets/b718fa3b-29f8-44c1-881d-6790490e6383" />

</p>

### Observation

- Minimal crossover distortion due to proper Class AB biasing.
- Output waveform remains nearly sinusoidal.
- Signal distortion is significantly lower than a Class B amplifier.

---
### Result

| Parameter | Value |
|-----------|-------|
| Efficiency | **47%** |

### Observation

- The amplifier achieves **47% efficiency**.
- Efficiency is significantly higher than a Class A amplifier.
- Provides a good balance between efficiency and signal fidelity.

---

# Results Summary

| Parameter | Result |
|-----------|--------|
| Amplifier Type | Class AB |
| Simulation Software | LTspice XVII |
| Analyses Performed | Transient, FFT, Distortion, Efficiency |
| Efficiency | **47%** |
| Output Quality | Low Distortion |
| Application | Audio Power Amplification |

---

#  Future Improvements

- PCB implementation
- Hardware implementation
- Higher output power design
