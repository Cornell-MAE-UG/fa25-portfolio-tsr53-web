---
layout: project
title: HW4 Portfolio
description: Additional Homework Question
technologies: N/a
image: /assets/images/IMA55DESIGN.png
---


# HW12 Portfolio Update 4 – IMA55 Actuator (35.8 kN)

For this update I redesigned my HW5 mechanism using the larger IMA55 actuator (max force 35.8 kN).  
The design space is 150 cm × 50 cm. I used a 120 cm bar, two ground pins, one bar pin for the actuator, and the load at the far end.

---

## Rigid-Bar Analysis

To get the basic geometry, I treated the bar as rigid.  
The actuator attaches at 0.40L and the load is at L.

Moment balance about A:

$$
F_{IMA} \cdot (0.40L) = W \cdot L
$$

So the maximum load is:

$$
W_{max} = 0.40 \times 35.8\ \text{kN} \approx 14.3\ \text{kN}
$$

This gives the theoretical lifting capacity before considering beam bending.

---

## Beam Deflection (Bar Not Rigid)

Now the bar is treated as a cantilever beam with length:

$$
L = 1.2\ \text{m}
$$

Loads applied:

- Tip load:  
  $$
  W = 14.3\ \text{kN}
  $$

- Actuator vertical component at  
  $$
  a = 0.40L
  $$

  Vertical force component:
  $$
  F_v = 35.8\ \text{kN}\ \sin(\theta)
  $$

### Tip deflection:

$$
\delta_W = \frac{W L^3}{3EI}
$$

### Actuator deflection:

$$
\delta_{act} = F_v \frac{a^2 (3L - a)}{6EI}
$$

### Total:

$$
\delta_{max} = \delta_W + \delta_{act} \le 0.02L = 0.024\ \text{m}
$$

This gives the stiffness requirement that the beam must satisfy.

---

## Final Beam Choice

To stay under the 2% deflection limit without making the design too heavy, I used a 6061-T6 rectangular hollow tube:

- 50 mm × 30 mm  
- 3 mm wall thickness  

This section provides enough moment of inertia to keep deflection within limits.

---

## Final Notes

The IMA55 actuator allowed a much larger load than my HW5 design.  
After that, the limiting factor became the beam stiffness rather than the actuator force, so the cross-section selection was more important.
