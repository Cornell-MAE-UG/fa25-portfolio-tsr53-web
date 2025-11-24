---
layout: project
title: Thermo HW11
description: Thermodynamic Analysis of a Piston Engine
technologies: N/a
image: assets/images/image_2025-11-24_152027144.png
---

# Thermodynamic Analysis of a Piston Engine

In November 2025, as part of a homework for a thermodynamics class I had to analyze a real thermodynamic system and consider ways to improve it.

---

## The Model of the Piston Engine

- The piston moves up and down inside the cylinder.  
- A connecting rod links the piston to the crankshaft, converting the piston’s reciprocating motion into shaft rotation.  
- Intake and exhaust valves in the cylinder head control the flow of air–fuel mixture into the cylinder and exhaust gases out.  
- A spark plug ignites the compressed mixture near top dead center (TDC).  
- Combustion gases exert high pressure on the piston crown, doing work on the piston and turning the crankshaft.

---

# The Engine Cycle

## Intake Stroke
- Piston moves from TDC to bottom dead center (BDC).  
- Intake valve open, exhaust valve closed.  
- Cylinder pressure slightly below ambient; fresh air–fuel mixture flows in.

## Compression Stroke
- Piston moves BDC → TDC.  
- Both valves closed.  
- Mixture is compressed; pressure and temperature rise (roughly adiabatically).

## Power Stroke (Combustion / Expansion)
- Near TDC, spark plug ignites the mixture.  
- Rapid combustion raises pressure and temperature.  
- High-pressure gas forces piston TDC → BDC, producing useful shaft work.

## Exhaust Stroke
- Exhaust valve opens.  
- Piston moves BDC → TDC, pushing exhaust gases out.

---

# Mass and Energy Balance

## Mass Balance
Mass in = Mass out  

---

## Energy Balance

For a steady-periodic piston engine cycle, the general energy balance is:

$$
\text{Power}_{\text{shaft}}
=
\dot{Q}_{\text{walls}}
+
\dot{m}\left( h_{\text{in}} - h_{\text{out}} \right)
$$

Where:

- \( \dot{Q}_{\text{walls}} \) = heat transfer through the cylinder walls  
- \( \dot{m} \) = mass flow rate  
- \( h_{\text{in}}, h_{\text{out}} \) = inlet and exit enthalpies  

---

## Performance Metrics

Thermal efficiency for a single-cylinder piston cycle can be expressed as:

$$
\eta = 
\frac{W_{\text{shaft}}}{Q_{\text{in}}}
$$

Where:

- \( W_{\text{shaft}} \) = net work delivered to the crankshaft  
- \( Q_{\text{in}} \) = heat added during combustion  

For idealized analysis (Otto cycle), efficiency depends on the compression ratio \( r \):

$$
\eta_{\text{otto}} = 1 - r^{\,1-\gamma}
$$

---

## Design Change: Increasing the Compression Ratio

A modification was made to increase the engine’s compression ratio:

- **Original compression ratio:** 8:1  
- **New compression ratio:** 11:1  

This reduces the clearance volume at top dead center, which:

- increases peak pressure and temperature,  
- improves thermal efficiency,  
- increases the mean effective pressure (MEP),  
- and results in more shaft work per cycle.

Geometric changes required:

- reshaping the piston crown,  
- reducing the combustion chamber clearance height,  
- preserving valve clearances to avoid mechanical interference.

---

## Summary

In this project, a simplified thermodynamic model of a piston engine was analyzed through:

- characterization of the four-stroke cycle,  
- application of mass and energy balances,  
- evaluation of thermal efficiency, and  
- implementation of a compression-ratio improvement strategy.

The design change demonstrates how small geometric modifications in the combustion chamber can meaningfully improve engine performance through increased pressure ratios and improved combustion efficiency.

