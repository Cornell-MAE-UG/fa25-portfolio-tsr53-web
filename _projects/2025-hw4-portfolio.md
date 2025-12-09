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

## Rigid-Bar Analysis

I treated the bar as rigid first to get the basic geometry.
The actuator attaches at $0.40L$ and the load is at $L$.
Moment balance about A:

$$
F_{\text{IMA}}(0.40L) = W L
$$

So,

$$
W_{\max} = 0.40 \times 35.8\,\text{kN} \approx 14.3\,\text{kN}
$$

This is the theoretical max load for the rigid case.

---

## Beam Deflection (Bar Not Rigid)

Now the bar is a cantilever beam ($L = 1.2\,\text{m}$).

Loads:

- Tip load: $W = 14.3\,\text{kN}$
- Actuator vertical component at $a = 0.40L$:
  $$
  F_v = 35.8\,\text{kN}\,\sin\theta
  $$

Tip deflection:

$$
\delta_W = \frac{W L^3}{3EI}
$$

Actuator deflection:

$$
\delta_{\text{act}} = F_v \frac{a^2(3L - a)}{6EI}
$$

Total:

$$
\delta_{\max} = \delta_W + \delta_{\text{act}} \le 0.02L = 0.024\,\text{m}
$$

This gives the stiffness requirement.

---

## Final Beam Choice

To meet the 2% deflection limit without adding unnecessary mass, I used a 6061-T6 rectangular hollow tube:

- $50\,\text{mm} \times 30\,\text{mm}$
- $3\,\text{mm}$ wall

This section gives enough $I$ to satisfy the stiffness target for all expected angles.

---

## Final Notes

The IMA55 force allowed much more load than my HW5 design.
The limiting factor ended up being beam stiffness, not actuator force, so picking an efficient cross-section mattered more than raw strength.
