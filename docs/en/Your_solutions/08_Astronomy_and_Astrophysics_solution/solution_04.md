## Problem 4: Geostationary Orbit

### Given / Knowns
* Earth's Mass, $M_E \approx 5.97 \times 10^{24} \text{ kg}$
* Earth's Radius, $R_E \approx 6378 \text{ km} = 6,378,000 \text{ m}$
* Universal Gravitational Constant, $G \approx 6.674 \times 10^{-11} \text{ N}\cdot\text{m}^2/\text{kg}^2$

### Concepts & Assumptions
* **Geostationary Period:** For a satellite to remain fixed above the exact same point on Earth's equator, its orbital period must perfectly match the Earth's rotational period. 
* **Assumption on Time:** We will use the standard 24-hour day for our calculations. (Note: Using the true sidereal day of 23 hours and 56 minutes yields a slightly more precise altitude of roughly 35,786 km, but 24 hours is standard for introductory physics derivations).
* **Deriving Kepler's Third Law:** We will find the orbital radius by equating the gravitational force to the centripetal force, substituting velocity $v$ with distance over time ($2\pi r / T$).

### Formulas
* Gravitational Force: $F_g = \frac{G M m}{r^2}$
* Centripetal Force: $F_c = \frac{m v^2}{r}$
* Circular Velocity: $v = \frac{2\pi r}{T}$
* Orbital Altitude: $h = r - R_E$

### Step-by-Step Derivation

**Part 1: The Orbital Period**
By definition, a geostationary satellite rotates synchronously with the Earth.
$$T = 24 \text{ hours} = 86400 \text{ seconds}$$

**Part 2: Calculating Orbital Radius ($r$)**
Set the gravitational force equal to the centripetal force required to keep the satellite in orbit:
$$\frac{G M_E m}{r^2} = \frac{m v^2}{r}$$

Cancel the satellite's mass ($m$) and simplify:
$$\frac{G M_E}{r} = v^2$$

Substitute the circular velocity formula $v = \frac{2\pi r}{T}$ into the equation:
$$\frac{G M_E}{r} = \left(\frac{2\pi r}{T}\right)^2$$
$$\frac{G M_E}{r} = \frac{4\pi^2 r^2}{T^2}$$

Rearrange the equation to solve for $r^3$ (this is a derivation of Kepler's Third Law):
$$r^3 = \frac{G M_E T^2}{4\pi^2}$$

Now, plug in the known values:
$$r^3 = \frac{(6.674 \times 10^{-11} \text{ N}\cdot\text{m}^2/\text{kg}^2)(5.97 \times 10^{24} \text{ kg})(86400 \text{ s})^2}{4\pi^2}$$
$$r^3 = \frac{(3.984 \times 10^{14})(7,464,960,000)}{39.478}$$
$$r^3 = \frac{2.974 \times 10^{24}}{39.478}$$
$$r^3 \approx 7.533 \times 10^{22} \text{ m}^3$$

Take the cube root to find $r$:
$$r = \sqrt[3]{7.533 \times 10^{22}}$$
$$r \approx 42,230,000 \text{ m} = 42,230 \text{ km}$$

**Part 3: Calculating Altitude ($h$)**
The radius $r$ is the distance from the *center* of the Earth. To find the altitude above the surface, subtract Earth's radius:
$$h = r - R_E$$
$$h = 42,230 \text{ km} - 6378 \text{ km}$$
$$h = 35,852 \text{ km}$$

### Final Answer
* The orbital period of a geostationary satellite must be **24 hours**.
* The altitude of a geostationary orbit is approximately **35,850 km** above the Earth's surface.