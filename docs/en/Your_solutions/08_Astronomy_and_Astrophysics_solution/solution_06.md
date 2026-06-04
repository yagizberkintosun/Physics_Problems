## Problem 6: Solar Gravity

### Given / Knowns
* Sun's Mass, $M_S \approx 2 \times 10^{30} \text{ kg}$
* Sun's Radius, $R_S \approx 6.96 \times 10^8 \text{ m}$
* Universal Gravitational Constant, $G \approx 6.674 \times 10^{-11} \text{ N}\cdot\text{m}^2/\text{kg}^2$
* Earth's Surface Gravity, $g_E \approx 9.81 \text{ m/s}^2$

### Concepts & Assumptions
* **Surface Gravity:** The acceleration due to gravity on the surface of any celestial body is derived from Newton's Law of Universal Gravitation, assuming a spherical mass distribution.
* **Weight vs. Mass:** An object's mass ($m$) is constant regardless of location. Its weight ($W$) is the force of gravity acting upon that mass ($W = mg$). Therefore, the factor by which your weight increases is exactly equal to the ratio of the Sun's surface gravity to Earth's surface gravity.

### Formulas
* Surface Gravity: $g = \frac{GM}{R^2}$
* Weight: $W = mg$
* Weight Factor: $\text{Factor} = \frac{W_S}{W_E} = \frac{m g_S}{m g_E} = \frac{g_S}{g_E}$

### Step-by-Step Derivation

**Part 1: Calculating Solar Gravity ($g_S$)**
Plug the known values for the Sun into the surface gravity formula:

$$g_S = \frac{G M_S}{R_S^2}$$
$$g_S = \frac{(6.674 \times 10^{-11} \text{ N}\cdot\text{m}^2/\text{kg}^2)(2 \times 10^{30} \text{ kg})}{(6.96 \times 10^8 \text{ m})^2}$$

First, simplify the numerator:
$$6.674 \times 10^{-11} \times 2 \times 10^{30} = 13.348 \times 10^{19}$$

Next, square the denominator:
$$(6.96 \times 10^8)^2 \approx 48.4416 \times 10^{16} = 4.84416 \times 10^{17}$$

Divide the numerator by the denominator:
$$g_S = \frac{13.348 \times 10^{19}}{4.84416 \times 10^{17}}$$
$$g_S \approx 275.55 \text{ m/s}^2$$

**Part 2: Calculating the Weight Increase Factor**
Now, determine how many times stronger this is compared to Earth's gravity:

$$\text{Factor} = \frac{g_S}{g_E}$$
$$\text{Factor} = \frac{275.55 \text{ m/s}^2}{9.81 \text{ m/s}^2}$$
$$\text{Factor} \approx 28.09$$

### Final Answer
* The acceleration due to gravity on the surface of the Sun is approximately **275.55 m/s²**.
* If you could stand on the Sun's surface, your weight would increase by a factor of roughly **28** (meaning you would feel about 28 times heavier than you do on Earth).