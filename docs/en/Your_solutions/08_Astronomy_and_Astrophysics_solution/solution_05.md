## Problem 5: Escape Velocity

### Given / Knowns
* Moon's Mass, $M_M \approx 7.35 \times 10^{22} \text{ kg}$
* Moon's Radius, $R_M \approx 1737 \text{ km} = 1,737,000 \text{ m}$
* Earth's Escape Velocity, $v_{e,\text{Earth}} \approx 11.2 \text{ km/s}$
* Universal Gravitational Constant, $G \approx 6.674 \times 10^{-11} \text{ N}\cdot\text{m}^2/\text{kg}^2$

### Concepts & Assumptions
* **Conservation of Energy:** To "escape" a celestial body's gravitational pull, a projectile must be launched with enough initial kinetic energy ($K$) to reach an infinite distance away, where its final kinetic energy and final gravitational potential energy ($U$) both approach zero.
* Total Initial Energy = Total Final Energy
* $K_i + U_i = K_f + U_f$
* $K_i + U_i = 0$

### Formulas
* Kinetic Energy: $K = \frac{1}{2}mv^2$
* Gravitational Potential Energy: $U = -\frac{GMm}{r}$
* Escape Velocity Derivation: $\frac{1}{2}mv_e^2 - \frac{GMm}{r} = 0 \implies v_e = \sqrt{\frac{2GM}{r}}$

### Step-by-Step Derivation

**Part 1: Calculating the Moon's Escape Velocity**
Using the derived formula for escape velocity, we plug in the values for the Moon (ensuring radius is in meters):

$$v_{e,\text{Moon}} = \sqrt{\frac{2 G M_M}{R_M}}$$
$$v_{e,\text{Moon}} = \sqrt{\frac{2 (6.674 \times 10^{-11} \text{ N}\cdot\text{m}^2/\text{kg}^2)(7.35 \times 10^{22} \text{ kg})}{1,737,000 \text{ m}}}$$

First, simplify the numerator:
$$2 \times 6.674 \times 10^{-11} \times 7.35 \times 10^{22} \approx 9.811 \times 10^{12}$$

Now divide by the radius:
$$v_{e,\text{Moon}} = \sqrt{\frac{9.811 \times 10^{12}}{1,737,000}}$$
$$v_{e,\text{Moon}} \approx \sqrt{5,648,244}$$
$$v_{e,\text{Moon}} \approx 2376.6 \text{ m/s}$$

Convert to km/s:
$$v_{e,\text{Moon}} \approx 2.38 \text{ km/s}$$

**Part 2: Fraction of Earth's Escape Velocity**
Now we compare the Moon's escape velocity to Earth's by setting up a ratio:

$$\text{Fraction} = \frac{v_{e,\text{Moon}}}{v_{e,\text{Earth}}}$$
$$\text{Fraction} = \frac{2.38 \text{ km/s}}{11.2 \text{ km/s}}$$
$$\text{Fraction} \approx 0.2125$$

### Final Answer
* The escape velocity from the surface of the Moon is approximately **2.38 km/s**.
* This is roughly **0.21 (or 21%)** of Earth's escape velocity.