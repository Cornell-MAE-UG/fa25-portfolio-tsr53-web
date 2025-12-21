---
layout: project
title: Thermo HW11
description: Thermodynamic Analysis of a Piston Engine
technologies: N/a
image: C:\Users\74975\Desktop\Statics GitHub\fa25-portfolio-tsr53-web\assets\images\dmrjskf.gif
---

Code

---
layout: project
title: Thermodynamic Analysis of a Piston Engine
description: Thermodynamic Analysis of the Engine
technologies: [Autodesk Fusion 360]
image: /assets/images/car-engine-CAD.png
---

In November 2025, as part of a homework for a thermodynamics class I had to analyze a real thermodynamic system and consider ways to improve it.

<br>
<br>
<br>


### The Model of the Engine

A piston-cylinder engine is a mechanical system that converts energy from a working fluid into reciprocating motion. It consists of a cylindrical chamber in which the piston moves back and forth (up and down) as pressure within the cylinder changes. In this analysis, the engine is modelled as an **Otto Cycle**, which consists of the following steps:

- **1 → 2:** Isentropic compression  
- **2 → 3:** Constant-volume heat addition  
- **3 → 4:** Isentropic expansion  
- **4 → 1:** Constant-volume heat rejection  

In this ideal case, all processes are assumed to be internally reversible, and there is no heat transfer between the system and the surroundings.

## The P-v Diagram

<img src="{{ '/assets/images/Pv_diagram.jpeg' | relative_url }}" alt="P-v Diagram" style="width:500px; max-width:100%; height:auto;">

## The T-s Diagram

<img src="{{ '/assets/images/Ts_diagram.jpeg' | relative_url }}" alt="T-s Diagram" style="width:500px; max-width:100%; height:auto;">

## Work and Heat for Each Process

<img src="{{ '/assets/images/QandW_Transfer.jpeg' | relative_url }}" alt="Work and Heat Equations" style="width:500px; max-width:100%; height:auto;">

The net work of the cycle is obtained by subtracting the work input during process **1 → 2** from the work output during process **3 → 4**. The net work can also be evaluated as the net heat added, which is found by subtracting the heat rejected during process **4 → 1** from the heat added during process **2 → 3**. Therefore, the area enclosed by both the **p–v diagram** and the **T–s diagram** represents the net work output of the ideal **Otto Cycle**.

Since air is assumed to behave as an ideal gas, the work and heat transfer for each process can be expressed in terms of the specific heat at constant volume. The work done or heat transferred during a process from state \(a \to b\) is proportional to \(c_v\) times the temperature change between the states.

## Control Mass Drawings for the System

<img src="{{ '/assets/images/FirstTwoSteps.jpeg' | relative_url }}" alt="First Two Steps" style="width:500px; max-width:100%; height:auto;">
<img src="{{ '/assets/images/LastTwoSteps.jpeg' | relative_url }}" alt="Last Two Steps" style="width:500px; max-width:100%; height:auto;">

---

## Mass Balance

### General control-volume form
$$
\frac{dm_{CV}}{dt} = \sum \dot{m}_{in} - \sum \dot{m}_{out}
$$

### For a piston engine
- Over a full cycle, the engine returns to its initial state.
- Therefore, there is **no net mass accumulation**.

$$
\sum \dot{m}_{in} = \sum \dot{m}_{out}
$$

---

## Energy Balance (First Law of Thermodynamics)

### General control-volume form
$$
\frac{dE_{CV}}{dt}
= \sum \dot{Q} - \sum \dot{W}
+ \sum \dot{m}_{in}\left(h + \frac{V^2}{2} + gz\right)_{in}
- \sum \dot{m}_{out}\left(h + \frac{V^2}{2} + gz\right)_{out}
$$

### For a piston engine (simplifications)
- Changes in kinetic and potential energy are negligible.
- Over a cycle, the system returns to its initial state:

$$
\frac{dE_{CV}}{dt} = 0
$$

So the cycle energy balance becomes:
$$
\sum \dot{Q} - \sum \dot{W} + \sum \dot{m}_{in}h_{in} - \sum \dot{m}_{out}h_{out} = 0
$$

This balance governs **engine efficiency and power output**.

---

## Entropy Balance (Second Law of Thermodynamics)

### General control-volume form
$$
\frac{dS_{CV}}{dt}
= \sum \frac{\dot{Q}_k}{T_k}
+ \sum \dot{m}_{in}s_{in}
- \sum \dot{m}_{out}s_{out}
+ \dot{S}_{gen}
$$

**Note:** \( \dot{S}_{gen} \ge 0 \)

### For steady cyclic operation
Over a full cycle, \(dS_{CV}/dt = 0\), so:
$$
\sum \frac{\dot{Q}_k}{T_k}
+ \sum \dot{m}_{in}s_{in}
- \sum \dot{m}_{out}s_{out}
+ \dot{S}_{gen} = 0
$$

The entropy balance quantifies **irreversibility and efficiency limits**.

---

We did this project in a group, and the people in my group were **Sanithu Mohottige** and **Panashe Neghna**.
