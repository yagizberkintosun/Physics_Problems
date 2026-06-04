## Problem 3: Microgravity

### Given / Knowns
* Altitude of ISS, $h = 400 \text{ km} = 400,000 \text{ m}$
* Earth's Mass, $M_E \approx 5.97 \times 10^{24} \text{ kg}$ (from standard reference/previous problem)
* Earth's Radius, $R_E \approx 6378 \text{ km} = 6,378,000 \text{ m}$
* Universal Gravitational Constant, $G \approx 6.674 \times 10^{-11} \text{ N}\cdot\text{m}^2/\text{kg}^2$

### Concepts & Assumptions
* **Acceleration Due to Gravity:** The acceleration due to gravity ($g$) at any point in space is determined by Newton's Law of Universal Gravitation. It depends on the mass of the central body (Earth) and the distance from its center.
* **Apparent Weight vs. True Weight:** True weight is the actual force of gravity acting on a mass ($F_g = mg$). Apparent weight is the normal force pushing back on an object. 

### Formulas
* Universal Gravitation: $F_g = \frac{G M m}{r^2}$
* Newton's Second Law: $F = m a$ (where $a$ becomes local gravity $g$)
* Derived Local Gravity Formula: $g = \frac{G M_E}{r^2}$ 
*(Note: $r$ is the total distance from Earth's center, so $r = R_E + h$)*

### Step-by-Step Derivation

**Part 1: Calculating Local Gravity ($g$)**
First, determine the total distance from the center of the Earth to the ISS ($r$):
$$r = R_E + h$$
$$r = 6,378,000 \text{ m} + 400,000 \text{ m} = 6,778,000 \text{ m}$$

Next, substitute the known values into the local gravity formula:
$$g = \frac{G M_E}{r^2}$$
$$g = \frac{(6.674 \times 10^{-11} \text{ N}\cdot\text{m}^2/\text{kg}^2)(5.97 \times 10^{24} \text{ kg})}{(6,778,000 \text{ m})^2}$$

Calculate the numerator and denominator:
$$g = \frac{3.984 \times 10^{14} \text{ N}\cdot\text{m}^2/\text{kg}}{4.594 \times 10^{13} \text{ m}^2}$$
$$g \approx 8.67 \text{ m/s}^2$$

**Part 2: Why do astronauts experience "weightlessness"?**
As calculated above, gravity at the altitude of the ISS is roughly $8.67 \text{ m/s}^2$ (about 88% as strong as it is on Earth's surface). Therefore, gravity has certainly not disappeared.

Astronauts experience a feeling of "weightlessness" because they, along with the ISS itself, are in a continuous state of **free fall** towards the Earth. 

However, because the ISS has such an enormous horizontal velocity (as calculated in Problem 2), the surface of the Earth curves away from them at the exact same rate that they are falling. Since the astronauts and the space station are falling at the same rate, there is no **normal force** pushing up against the astronauts' feet (or bodies). The human sensation of "weight" comes from feeling this normal force pushing against us. Without a normal force, the apparent weight is zero, resulting in the sensation of weightlessness.

### Final Answer
* The acceleration due to gravity ($g$) at the altitude of the ISS is approximately **8.67 m/s²**.
* Astronauts experience weightlessness because they are in continuous **free fall**; lacking a supportive surface, there is no **normal force** to provide the physical sensation of weight.