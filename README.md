# Karaoke / Mixer Audio Device 🎶

**Course:** EE 210 – Spring 2025  
**Author:** Sadid Hassan  

> ⚡ **Note:** This README is a condensed version of my full course project report.  
> It highlights the design, simulation, and implementation of each block with figures.  
> For in-depth theory, derivations, and detailed calculations, please see the  
> [📄 Full Project Report (PDF)](docs/FinalReport.docx).

This project implements a **tone-control karaoke/mixer system** with real-time **volume, bass, and treble adjustment**, designed and simulated in **Multisim**, laid out in **Ultiboard**, and implemented on both **breadboard and PCB**.

---

## 📝 Overview
The system consists of five blocks:
1. **Mixer / Karaoke** – Combines or subtracts left/right audio inputs.  
2. **Tone Control** – Baxandall circuit for bass and treble adjustment.  
3. **Volume Control** – Potentiometer-based voltage divider.  
4. **Volume Display** – LED comparator circuit showing volume levels.  
5. **Attenuator & Output Buffer** – Prepares output for headphones/audio devices.  

Each block was designed, simulated, and tested individually, then integrated into a complete system.

---

## 🔧 Tools & Equipment
- **Software:** Multisim, Ultiboard  
- **Lab Tools:** NI MyDAQ, NI ELVISmx, Oscilloscope, DMM, Power Supply  
- **Hardware:** Op-amps, potentiometers, resistors, capacitors, SPDT switch, LEDs, breadboard, PCB  

---

## 📐 Block Designs

### Block 1: Mixer / Karaoke
- Implements both a **summing amplifier** (mixing mode) and **subtracting amplifier** (karaoke mode).  
- Switch determines operation:  
  - Mixer: `–(L+R)`  
  - Karaoke: `L – R`  

**Schematic**  
![Block 1 Schematic](images/Figure1.jpg)  

**Simulation Results**  
- Mixer Mode  
  ![Block 1 Mixer Mode](images/Figure2.jpg)  
- Karaoke Mode  
  ![Block 1 Karaoke Mode](images/Figure3.jpg)  

---

### Block 2: Tone Control
- Baxandall tone-control circuit for bass/treble adjustment.  
- RC filters allow user to boost or attenuate low and high frequencies.  

**Schematic**  
![Block 2 Schematic](images/Figure4.jpg)  

**Simulation Results**  
- Bass Boost  
  ![Bass Boost](images/Figure5.jpg)  
- Treble Boost  
  ![Treble Boost](images/Figure6.jpg)  
- Bass & Treble Attenuation  
  ![Bass + Treble Attenuation](images/Figure7.jpg)  

---

### Block 3: Volume Control
- 100kΩ potentiometer as a **voltage divider**.  
- Provides smooth control from **0 → max volume**.  

**Schematic**  
![Volume Control](images/Figure8.jpg)  

**Simulation Result**  
![Volume Simulation](images/Figure9.jpg)  

---

### Block 4: Volume Display
- Uses **comparator op-amps** with resistor ladder reference voltages.  
- Four LEDs light at different thresholds (0.25V, 0.5V, 1.0V, 1.5V).  

**Schematic**  
![Volume Display](images/Figure10.jpg)  

**Simulation Result**  
![LED Display Simulation](images/Figure11.jpg)  

---

### Block 5: Attenuator & Output Buffer
- Inverting op-amp stage reduces amplitude to **0.5–1V range**.  
- Prepares signal for **headphones or audio jacks**.  

**Schematic**  
![Attenuator Circuit](images/Figure12.jpg)  

**Simulation Result**  
![Attenuator Output](images/Figure13.jpg)  

---

## 🛠️ Implementation

**Breadboard Build**  
![Breadboard](images/Figure14.jpg)  

**PCB Build**  
![PCB](images/Figure15.jpg)  

**Complete Circuit Schematic**  
![Complete Schematic](images/Figure16.jpg)  

---

## ✅ Results & Conclusion
- Successfully built a **fully functional karaoke/mixer system** with bass, treble, volume, and LED display.  
- Learned practical applications of **op-amps, RC filters, comparators, and PCB design**.  
- Debugged issues such as grounding errors and LED activation thresholds, improving troubleshooting skills.  
- Project required integration of concepts from across the semester, reinforcing **circuit design, simulation, and system validation**.  

---

