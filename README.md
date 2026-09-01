# Soft Pneumatic Bending Actuator — DRDO

## Project Description

This project presents the design and development of a **bio-inspired pneumatically actuated soft robotic gripper** for adaptive and safe object handling. Inspired by the bending mechanism of a **lobster tail**, the Soft Pneumatic Bending Actuator (SPBA) combines a flexible silicone body with a rigid **kirigami-patterned shell** to convert pneumatic pressure into controlled bending motion.

The project integrates **CAD modelling, ANSYS finite element analysis (FEA), 3D-printed mould fabrication, silicone casting, and kirigami-based structural design** to investigate the relationship between actuator geometry, pressure, deformation, and bending performance.

The optimized **2.25 mm finger configuration** remained stable up to **39.84 kPa** and achieved a maximum simulated bending angle of **132.1°**. The actuator has an approximate weight of **22 g** and demonstrated a **600 g payload**.

---

## Project Overview

Soft robotics uses flexible and compliant materials to achieve large deformation and safer interaction with objects compared with conventional rigid mechanisms. This makes soft actuators particularly suitable for handling objects that are fragile, irregular, or variable in shape.

The developed actuator is designed around a bio-inspired bending mechanism. The concept is based on the lobster tail, where soft internal structures interact with relatively rigid external segments to produce controlled bending.

The developed **Soft Pneumatic Bending Actuator (SPBA)** uses:

- A soft silicone-based actuator body
- Dragon Skin and Ecoflex elastomers
- A rigid kirigami-patterned shell
- Pneumatic pressure for actuation
- 3D-printed moulds for fabrication
- CAD-based design and modelling
- ANSYS-based nonlinear FEA for optimization

---

## Objectives

The major objectives of the project are:

1. **Hardware Development**
   - Develop a three/four-finger soft robotic gripper concept using pneumatically actuated soft bending actuators.

2. **CAD-Based Design**
   - Develop detailed CAD models of the actuator and mould components suitable for fabrication.

3. **FEA Analysis**
   - Analyze pressure-induced deformation and bending behaviour using finite element analysis.

4. **Design Optimization**
   - Investigate the influence of actuator/finger thickness on structural stability, deformation, and bending angle.

5. **Experimental & Operational Evaluation**
   - Evaluate the actuator for handling structured and unstructured objects while considering payload, weight, and power requirements.

---

## Bio-Inspired Actuator Concept

The actuator design is inspired by the **lobster-tail mechanism**, where compliant structures and rigid segments work together to produce bending.

The developed SPBA consists of a hybrid structure:

**Soft Silicone Body + Rigid Kirigami Shell**

The silicone body is fabricated using **Dragon Skin and Ecoflex**, while the outer constraint structure incorporates a patterned kirigami shell.

### Working Principle

When compressed air is supplied to the actuator:

1. Pneumatic pressure is applied inside the soft chamber.
2. The silicone body tends to expand.
3. The kirigami shell restricts radial expansion.
4. The restricted expansion is converted into axial deformation.
5. The actuator bends in a controlled direction.
6. Increasing pressure produces a greater bending angle within the stable operating range.

The actuator length used in the design is approximately **110 mm**.

---

## Actuator Performance

The developed actuator demonstrated a lightweight design with significant payload capability.

| Parameter | Value |
|---|---:|
| Actuator Length | ~110 mm |
| Actuator Weight | ~22 g |
| Payload | ~600 g |
| Power-to-Weight Ratio | ~27.27× |

These performance values are reported in the project design documentation.

---

## Design & CAD Modelling

The actuator and mould components were designed using CAD modelling techniques before fabrication.

The CAD development included:

- Soft actuator geometry
- Kirigami constraint structure
- Mould components
- Top and bottom mould sections
- Base components
- Assembly-related features

The CAD models were developed with fabrication requirements in mind, allowing the mould components to be manufactured using additive manufacturing.

---

## Finite Element Analysis

FEA was performed in **ANSYS** to investigate the nonlinear deformation behaviour of the soft actuator.

Because silicone elastomers undergo large deformation and exhibit nonlinear material behaviour, a **Mooney–Rivlin hyperelastic material model** was used.

### ANSYS Setup

| Parameter | Value |
|---|---:|
| Material | Silicone Rubber / Ecoflex-type elastomer |
| Material Model | Mooney–Rivlin |
| Element Size | 3 mm |
| Number of Steps | 15 |
| C01 | 259 kPa |
| C10 | 65 kPa |
| Incompressibility | 10⁻⁶ kPa⁻¹ |
| Density | 1100 kg/m³ |

The selected material model accounts for large elastic deformation, nonlinear stress–strain behaviour, and near-incompressibility of the silicone elastomer. 

---

## Thickness Optimization

Different finger thicknesses were investigated using FEA to understand their influence on deformation and pressure capability.

### 2.25 mm Finger Thickness

- Stable up to **39.84 kPa**
- Maximum deflection: **0.0704 m**
- Nodes: **72,328**
- Elements: **41,160**
- Maximum bending angle: **132.1°**

Beyond the stable pressure range, excessive deformation and distortion of the finger geometry were observed.

### 2.00 mm Finger Thickness

- Stable up to **23.34 kPa**
- Maximum deflection: **0.11492 m**
- Nodes: **66,349**
- Elements: **37,318**
- Maximum bending angle: **59.9°**

Excessive deformation occurred beyond the stability threshold. 

### 1.75 mm Finger Thickness

- Stable up to **20.80 kPa**
- Maximum deflection: **0.15066 m**
- Nodes: **111,396**
- Elements: **69,535**
- Maximum bending angle: **78.5°**

Further pressure resulted in excessive deformation and distortion of the actuator geometry.

---

## Pressure–Bending Response

The FEA results demonstrate the relationship between applied pneumatic pressure and actuator bending angle.

| Finger Thickness | Pressure | Bending Angle |
|---|---:|---:|
| **2.25 mm** | 10 kPa | 15.2° |
| | 20 kPa | 36.8° |
| | 30 kPa | 65.1° |
| | 35 kPa | 92.4° |
| | 39.84 kPa | **132.1°** |
| **2.00 mm** | 5 kPa | 8.8° |
| | 10 kPa | 20.7° |
| | 15 kPa | 35.0° |
| | 20 kPa | 51.2° |
| | 23.34 kPa | **59.9°** |
| **1.75 mm** | 5 kPa | 13.8° |
| | 10 kPa | 32.5° |
| | 15 kPa | 53.6° |
| | 20 kPa | 74.2° |
| | 20.80 kPa | **78.5°** |

The project results show that **finger thickness significantly affects pressure tolerance, deformation, and bending behaviour**.
---

## 3D-Printed Mould Fabrication

The moulds required for fabricating the soft actuator were manufactured using **Fused Deposition Modeling (FDM)**.

### Manufacturing Process

- **Manufacturing method:** FDM 3D printing
- **Material:** PLA
- **Slicing software:** Ultimaker Cura
- **Purpose:** Fabrication of mould components for silicone casting
- **Printing principle:** Layer-by-layer material deposition

The project used Ultimaker Cura to prepare the models and generate the G-code required for 3D printing. 

---

## Slicing of Mould

The CAD mould components were prepared for additive manufacturing using **Ultimaker Cura**.

Separate slicing operations were performed for:

- Base Part
- Bottom Part
- Top Part

The slicing stage was used to prepare the mould geometry for FDM fabrication and generate the required toolpath/G-code.

---

## Fabrication Methodology

The soft actuator fabrication followed a multi-stage process.

### 1. Mould Fabrication

3D-printed moulds were designed using CAD software and manufactured to create the required soft-body geometry.

### 2. Soft Body Casting

Two silicone elastomers, **Dragon Skin 30** and **Ecoflex 00-30**, were used to form the bilayer soft structure.

### 3. Layer Bonding

The inner and outer silicone layers were chemically bonded during curing to achieve seamless integration.

### 4. Kirigami Shell Preparation

Thin rigid sheets were laser-cut with strategically designed patterns to create the constraint shell.

### 5. Final Assembly

After curing, the soft body was inserted into the kirigami shell and end caps were attached to seal the actuator chambers.

### 6. Inlet Integration

Air inlet tubes were integrated during casting to provide pneumatic actuation and controlled pressure input.

This fabrication sequence is documented in the project fabrication methodology.

---

## Materials

### Soft Actuator

- Dragon Skin 30
- Ecoflex 00-30

### Mould

- PLA
- FDM 3D printing

### Constraint Structure

- Thin rigid sheet
- Laser-cut kirigami pattern

### Pneumatic System

- Air inlet tubing
- Pressurized air source

---

## Technology & Tools

| Category | Tools / Technology |
|---|---|
| CAD Design | Creo |
| Simulation | ANSYS |
| FEA | Nonlinear Hyperelastic Analysis |
| Slicing | Ultimaker Cura |
| Manufacturing | FDM 3D Printing |
| Mould Material | PLA |
| Actuator Material | Dragon Skin + Ecoflex |
| Actuation | Pneumatic Pressure |

---

## Key Results

The project demonstrated the feasibility of a **lightweight, high-deformation pneumatic soft actuator** for adaptive robotic manipulation.

### Major findings

- A hybrid **soft-rigid architecture** can convert pneumatic expansion into controlled bending.
- Finger thickness has a significant influence on structural stability and bending response.
- The **2.25 mm configuration** demonstrated the highest stable pressure range among the investigated configurations.
- A maximum simulated bending angle of **132.1°** was obtained at **39.84 kPa** for the 2.25 mm configuration.
- The actuator achieved an approximate **600 g payload with a mass of only ~22 g**.
- CAD and 3D printing enabled rapid fabrication of the required mould components.
- FEA provided a basis for understanding the pressure–deformation relationship and selecting suitable actuator geometry.

---

## Applications

The developed soft gripper/actuator concept can be applied to situations requiring compliant and adaptive interaction with objects, including:

- Robotic object manipulation
- Handling fragile objects
- Handling irregularly shaped objects
- Industrial automation
- Robotic gripping systems
- Tool and handle manipulation
- Hose manipulation
- Adaptive grasping

Soft robotic systems are particularly useful where conventional rigid grippers may cause damage or have difficulty adapting to different object geometries. 

---

## Project Workflow

```text
Concept Development
        ↓
Bio-Inspired Actuator Design
        ↓
CAD Modelling
        ↓
FEA & Design Optimization
        ↓
Mould Design
        ↓
3D Printing of Mould
        ↓
Silicone Casting
        ↓
Layer Bonding & Curing
        ↓
Kirigami Shell Fabrication
        ↓
Final Assembly
        ↓
Pneumatic Actuation
        ↓
Performance Evaluation
