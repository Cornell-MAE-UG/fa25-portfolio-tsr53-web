---
layout: project
title: HW4 Portfolio
description: Additional Homework Question
technologies: N/a
image: /assets/images/IMA55DESIGN.png
---


# HW12 Portfolio Update – IMA55 Actuator (35.8 kN)

For this update I redesigned my HW5 mechanism using the larger IMA55 actuator (max force 35.8 kN).  
The design space is 150 cm × 50 cm. I used a 120 cm bar, two ground pins, one bar pin for the actuator, and the load at the far end.

---

## Rigid-Bar Analysis

I treated the bar as rigid to get the basic geometry.  
The actuator attaches at \(0.40L\) and the load is at \(L\).

Moment balance about A:

$$
F_{\text{IMA}} (0.40L) = W L
$$

So the max load is:

$$
W_{\max} = 0.40 \times 35.8 \text{ kN} \approx 14.3 \text{ kN}
$$

This gives the theoretical lifting capacity before considering beam bending.

---

## Beam Deflection (Bar Not Rigid)

Now the bar is considered as a cantilever beam of length \(L = 1.2 \text{ m}\).

Loads:

- Tip load: \(W = 14.3 \text{ kN}\)
- Actuator vertical force component at \(a = 0.40L\):

$$
F_v = 35.8 \text{ kN} \cdot \sin(\theta)
$$

Tip deflection from the point load:

$$
\delta_W = \frac{W L^3}{3EI}
$$

Deflection from actuator force at an interior point:

$$
\delta_{\text{act}} = F_v \frac{a^2 (3L - a)}{6EI}
$$

Total deflection:

$$
\delta_{\max} = \delta_W + \delta_{\text{act}} \le 0.02L = 0.024 \text{ m}
$$

This inequality gives the stiffness requirement for the bar.

---

## Final Beam Choice

To stay under the 2% deflection limit while keeping mass low, I used a 6061-T6 aluminum hollow rectangular tube:

- \(50 \text{ mm} \times 30 \text{ mm}\)
- \(3 \text{ mm}\) wall thickness

This section provides enough \(I\) to keep deflection within limits for all expected actuator angles.

---

## Final Notes

The IMA55 actuator allowed a much larger load than my HW5 design.  
Once the actuator force was sufficient, the limiting factor became beam stiffness rather than strength, so the cross-section choice mattered most.

