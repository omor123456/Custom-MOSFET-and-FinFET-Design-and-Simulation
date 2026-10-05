# Custom MOSFET & FinFET Device Simulation

3D semiconductor device modeling and electrical characterization of planar MOSFET and FinFET structures using Synopsys Sentaurus TCAD.

---

### Overview

Modeled and simulated nanoscale MOSFET and FinFET devices in Sentaurus by defining semiconductor geometry, gate oxide, source/drain regions, and doping profiles.

The project focused on comparing the electrical behavior of a traditional planar MOSFET with a 3D FinFET using Id–Vg characteristics and threshold voltage measurements.

The simulation workflow included:

    Device Geometry
          ↓
    Doping Profiles
          ↓
    Mesh Refinement
          ↓
    Sentaurus Device Simulation
          ↓
    Gate Voltage Sweep
          ↓
    Id–Vg Characterization
          ↓
    MOSFET vs FinFET Analysis

---

### Device Structures

Both devices were modeled with nanoscale dimensions and comparable doping conditions to evaluate the effect of device geometry on electrostatic gate control.

MOSFET

• Planar silicon channel  
• 12 nm channel length  
• 2.5 nm gate oxide  
• 35 nm nominal source/drain width  
• Boron-doped bulk  
• Arsenic-doped source/drain regions  
• Gaussian source/drain doping profiles  

FinFET

• 3D fin-shaped silicon channel  
• 12 nm channel length  
• 2.5 nm gate oxide  
• 35 nm nominal source/drain width  
• Boron-doped bulk  
• Arsenic-doped source/drain regions  
• Gaussian source/drain doping profiles  

---

### Sentaurus TCAD Modeling

Used Sentaurus Structure Editor (SDE) to define the device geometry and semiconductor doping profiles.

The source and drain regions were modeled using Gaussian doping profiles, while the mesh was refined near the semiconductor/oxide interface to accurately capture the behavior of the thin gate oxide and channel region.

The device structures were then simulated using Sentaurus Device (SDevice).

Simulation files for both MOSFET and FinFET structures are included in the repository.

---

### Electrical Characterization

Measured the drain current as a function of gate voltage by sweeping:

    Vg = 0 V → 1 V

The Id–Vg characteristics were used to compare transistor turn-on behavior and threshold voltage between the planar MOSFET and FinFET.

Measured threshold voltages:

    MOSFET   → Vth ≈ 0.54 V
    FinFET   → Vth ≈ 0.26 V

The FinFET exhibited a steeper increase in drain current with increasing gate voltage compared with the planar MOSFET.

![MOSFET vs FinFET Id-Vg Characteristics](mosfet-vs-finfet-id-vg.png)

---

### MOSFET vs FinFET

The main difference observed in the simulation was the stronger gate control of the FinFET structure.

A planar MOSFET controls the channel primarily from the top surface through the gate oxide.

A FinFET uses a three-dimensional fin-shaped channel with the gate surrounding multiple sides of the channel. This provides stronger electrostatic control over the channel.

The resulting Id–Vg comparison demonstrated:

• Steeper drain-current increase in the FinFET  
• Lower simulated threshold voltage for the FinFET  
• Stronger gate-to-channel coupling  
• Improved electrostatic control of the channel  

These characteristics are important for scaling transistor dimensions while maintaining effective control of the conducting channel.

The SDE files contain the device structure and doping setup, while the SDevice files contain the electrical device simulation configuration.

---

### Tools

Synopsys Sentaurus TCAD  
3D semiconductor device modeling and simulation

Sentaurus Structure Editor (SDE)  
Device geometry, doping profiles, and mesh setup

Sentaurus Device (SDevice)  
Electrical simulation and Id–Vg characterization

---

### Skills Demonstrated

Semiconductor Device Modeling  
MOSFET Physics  
FinFET Physics  
TCAD Simulation  
3D Device Modeling  
Gaussian Doping Profiles  
Mesh Refinement  
Threshold Voltage Extraction  
Id–Vg Characterization  
Gate Electrostatic Control  
Device Structure Analysis

---

### Project Context

This project was completed as part of an ECE semiconductor device simulation assignment focused on modeling nanoscale MOSFET and FinFET structures in Sentaurus TCAD.

The project provided hands-on experience with the relationship between transistor geometry, doping, gate control, and electrical characteristics.

The final analysis compared the simulated Id–Vg behavior and threshold voltage of planar MOSFET and FinFET devices.
