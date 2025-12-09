---
layout: project
title: Thermo HW11
description: Thermodynamic Analysis of a Piston Engine
technologies: N/a
image: C:\Users\74975\Desktop\Statics GitHub\fa25-portfolio-tsr53-web\assets\images\dmrjskf.gif
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

## Energy Balance
\[
\text{Power}_{\text{shaft}} = \dot{Q}_{\text{walls}} 
  + \dot{m} \left( h_{\text{in}} - h_{\text{out}} \right)
\]

---

# Performance Metrics

For a piston engine cylinder operating in steady periodic cycles, the thermal efficiency can be written in the simplest form as:

\[
\eta = \frac{\text{work done by shaft}}{\text{heat in}}
\]

---

# Design Change

Increase the **compression ratio** (how much the engine squeezes the air–fuel mixture).

- **Baseline engine:** 8:1 compression  
- **New design:** 11:1 compression  

This is achieved by reducing the clearance volume at top dead center (changing piston/head geometry).
