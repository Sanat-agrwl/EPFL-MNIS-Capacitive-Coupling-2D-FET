# Capacitive Coupling in 2D FET

## Project Overview

This project investigates the phenomenon of capacitive coupling in a two-dimensional Field Effect Transistor (2D FET) architecture. Capacitive coupling is a critical effect in nanoscale devices where electrical fields from one structure can influence neighboring structures, affecting device performance and reliability.

### Objectives

- **Understand capacitive coupling mechanisms** in 2D FET structures at the nanoscale
- **Model and simulate** the electric field distribution using COMSOL Multiphysics
- **Analyze** the coupling effects between adjacent gates, channels, and substrates
- **Quantify** the capacitance contributions and their impact on device behavior
- **Develop insights** for designing low-power and high-performance transistor devices

## Problem Statement

In modern 2D materials-based transistors (such as those using graphene, MoS₂, or similar materials), capacitive coupling between different structural components leads to:
- Parasitic capacitances affecting switching speed
- Cross-talk between different gate regions
- Modified electric field distribution in the channel
- Implications for device scaling and performance

This project models these effects to better understand the relationship between device geometry, material properties, and coupling behavior.

## Methodology

The analysis is performed using **COMSOL Multiphysics**, which solves the Poisson equation for the electrostatic potential in the device structure. Key aspects include:

1. **Domain Definition**: 2D cross-section of the FET structure
2. **Boundary Conditions**: Applied voltages to gates, channels, and substrates
3. **Material Properties**: Permittivity values for different materials
4. **Simulation**: Electrostatic field analysis to compute potential distribution
5. **Post-processing**: Extraction of capacitances and field analysis

## Files in This Repository

- **14-Model.mph** - COMSOL Multiphysics physics-informed model of the 2D FET system
- **14-Report.pdf** - Detailed technical report with results, analysis, and conclusions
- **14-Presentation.pdf** - Presentation slides summarizing key findings
- **Project 14 - Capacitive coupling in 2D FET.pdf** - Project description and requirements
- **README.md** - This file

## Key Results

The simulation study provides insights into:
- Capacitive coupling strength between different device regions
- Electric field distribution under various bias conditions
- Scaling effects of device dimensions on coupling
- Design considerations for minimizing unwanted coupling effects

## How to Use the COMSOL Model

### Prerequisites
- COMSOL Multiphysics (version 5.5 or later recommended)
- Sufficient computational resources for 2D FET physics simulations

### Opening and Running the Model
1. Open COMSOL Multiphysics
2. File → Open → Select `14-Model.mph`
3. Review the geometry, materials, and physics settings
4. To run simulations: Study → Compute
5. Analyze results in the post-processing environment

### Modifying the Model
The model can be modified to:
- Change device geometry (gate length, width, material thickness)
- Adjust applied voltages and boundary conditions
- Explore different material systems
- Refine mesh for increased accuracy

## Technical Details

### Device Structure
- **Channel Material**: 2D semiconducting material (e.g., MoS₂, WSe₂, or graphene)
- **Gate Dielectric**: High-κ insulating material (typically SiO₂ or HfO₂)
- **Size Scale**: Nanometer to sub-100nm dimensions typical for 2D FETs

### Physics Solved
- **Electrostatics**: Poisson's equation in electrostatic form
- **Field Computation**: Electric field distribution and potential
- **Capacitance Extraction**: Methods include energy-based and field-based approaches

## References and Context

This project is part of the **EPFL Physical models for micro and nanosystems** course, focusing on device physics and simulation at the nanoscale.

## Author

**Project**: EPFL - Capacitive Coupling in 2D FET  
**Institution**: École Polytechnique Fédérale de Lausanne (EPFL)  
**Course**: Physical models for micro and nanosystems

## Notes

- All simulations assume equilibrium conditions unless otherwise specified
- Results should be validated against experimental measurements when available
- The 2D model simplification may not capture all out-of-plane effects present in real 3D devices
- For detailed explanation of results and interpretation, refer to **14-Report.pdf**

---

*For questions or further information, refer to the project documentation.*