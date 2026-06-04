## Problem 2: Orbital Mechanics

### Given / Knowns
**For the ISS:**
* Altitude of ISS, $h = 400 \text{ km} = 400,000 \text{ m}$
* Earth's Mass, $M_E \approx 5.97 \times 10^{24} \text{ kg}$
* Earth's Radius, $R_E \approx 6378 \text{ km} = 6,378,000 \text{ m}$ (from Problem 1 context)
* Universal Gravitational Constant, $G \approx 6.674 \times 10^{-11} \text{ N}\cdot\text{m}^2/\text{kg}^2$

**For Earth:**
* Earth-Sun distance (orbital radius), $R_{ES} \approx 150 \times 10^6 \text{ km}$
* Earth's orbital period, $T \approx 365.25 \text{ days}$

### Concepts & Assumptions
* **Orbital Velocity (Dynamic Approach):** For a satellite (like the ISS) to stay in a circular orbit, the gravitational pull of the Earth must exactly provide the necessary centripetal force required for circular motion. We assume a perfectly circular orbit for simplicity.
* **Orbital Velocity (Kinematic Approach):** For the Earth orbiting the Sun, we are given the distance and the time (period). Assuming a circular orbit, the speed is simply the total distance of the orbital path (circumference) divided by the time it takes to complete one orbit.
* **Assumption on Orbital Radii:** The orbital radius is measured from the *center* of the massive body. Therefore, the orbital radius of the ISS is the radius of the Earth *plus* the altitude of the ISS ($r = R_E + h$). 

### Formulas
* Gravitational Force: $F_g = \frac{G M m}{r^2}$
* Centripetal Force: $F_c = \frac{m v^2}{r}$
* Derived Orbital Speed (by setting $F_g = F_c$): $v = \sqrt{\frac{G M}{r}}$
* Average Speed for Circular Orbit: $v = \frac{2\pi r}{T}$

### Step-by-Step Derivation

**Part 1: Orbital Speed of the ISS**
First, calculate the orbital radius $r_{ISS}$ from the center of the Earth:
$$r_{ISS} = R_E + h$$
$$r_{ISS} = 6,378,000 \text{ m} + 400,000 \text{ m} = 6,778,000 \text{ m}$$

Now, set gravitational force equal to centripetal force to derive the velocity formula:
$$\frac{G M_E m_{ISS}}{r_{ISS}^2} = \frac{m_{ISS} v_{ISS}^2}{r_{ISS}}$$
$$v_{ISS}^2 = \frac{G M_E}{r_{ISS}}$$
$$v_{ISS} = \sqrt{\frac{G M_E}{r_{ISS}}}$$

Plug in the known values (using standard SI units):
$$v_{ISS} = \sqrt{\frac{(6.674 \times 10^{-11} \text{ N}\cdot\text{m}^2/\text{kg}^2)(5.97 \times 10^{24} \text{ kg})}{6,778,000 \text{ m}}}$$
$$v_{ISS} = \sqrt{\frac{3.984 \times 10^{14}}{6,778,000}}$$
$$v_{ISS} \approx \sqrt{5.878 \times 10^7} \approx 7667 \text{ m/s}$$
Convert to km/s:
$$v_{ISS} \approx 7.67 \text{ km/s}$$

**Part 2: Earth's Orbital Speed Around the Sun**
First, convert the period $T$ from days to seconds:
$$T = 365.25 \text{ days} \times 24 \frac{\text{h}}{\text{day}} \times 3600 \frac{\text{s}}{\text{h}}$$
$$T = 31,557,600 \text{ s}$$

Now use the kinematic formula for circular speed:
$$v_E = \frac{2\pi R_{ES}}{T}$$
$$v_E = \frac{2\pi (150 \times 10^6 \text{ km})}{31,557,600 \text{ s}}$$
$$v_E = \frac{942,477,796 \text{ km}}{31,557,600 \text{ s}}$$
$$v_E \approx 29.86 \text{ km/s}$$

### Final Answer
* The orbital speed of the ISS is approximately **7.67 km/s**.
* Earth's orbital speed around the Sun is approximately **29.86 km/s**.
* **Comparison:** The Earth moves much faster in its orbit around the Sun than the ISS moves in its orbit around the Earth.