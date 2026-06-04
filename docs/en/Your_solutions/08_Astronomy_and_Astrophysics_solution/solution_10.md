## Problem 10: Measuring the Height of the Atmosphere

### Given / Knowns
* Time between sunset and twilight ending, $t = 40 \text{ minutes}$
* Earth's radius, $R_E = 6370 \text{ km}$
* Earth's rotation rate = $360^\circ$ per 24 hours
* Geometric model formula: $\cos \phi = \frac{R_E}{R_E + h}$

### Concepts & Assumptions
* **Earth's Rotation:** The Earth rotates uniformly, completing a full $360^\circ$ rotation every 24 hours. By finding the rate of rotation in degrees per minute, we can determine exactly how far the Sun appears to drop below the horizon (the solar depression angle, $\phi$) during the 40-minute twilight period.
* **Geometric Model:** The "sharp-edge atmosphere" model assumes twilight ends exactly when the Sun's rays can no longer graze the surface of the Earth and hit the top of the atmosphere directly above the observer. This creates a right triangle connecting the Earth's center, the observer on the surface, and the top of the atmosphere where the ray grazes it.

### Formulas
* Angular Velocity (Rotation Rate): $\omega = \frac{\Delta \theta}{\Delta t}$
* Solar Depression Angle: $\phi = \omega \times t$
* Atmospheric Height (derived from given equation): $h = \frac{R_E}{\cos \phi} - R_E$

---

### Step-by-Step Derivation

#### 1. The solar depression angle $\phi$
First, calculate the Earth's rotational rate ($\omega$) in degrees per minute. We know the Earth rotates $360^\circ$ in 24 hours. Convert 24 hours to minutes:

$$24 \text{ hours} \times 60 \frac{\text{min}}{\text{hour}} = 1440 \text{ minutes}$$

Now, find the degrees rotated per minute:

$$\omega = \frac{360^\circ}{1440 \text{ min}} = 0.25^\circ / \text{min}$$

Since the faint stars appeared 40 minutes after sunset, we multiply this rate by the elapsed time to find the depression angle:

$$\phi = 0.25^\circ / \text{min} \times 40 \text{ min}$$

$$\phi = 10^\circ$$

#### 2. The atmospheric height $h$
Now that we have the angle $\phi$, we can use Al-Zarqali's geometric model to solve for $h$. We start with the given formula:

$$\cos \phi = \frac{R_E}{R_E + h}$$

Rearrange the equation to solve for $R_E + h$:

$$R_E + h = \frac{R_E}{\cos \phi}$$

Subtract $R_E$ from both sides to isolate $h$:

$$h = \frac{R_E}{\cos \phi} - R_E$$

Now, plug in the known values for $R_E$ and $\phi$:

$$h = \frac{6370 \text{ km}}{\cos(10^\circ)} - 6370 \text{ km}$$

Calculate the cosine of $10^\circ$ (ensure your calculator is in degree mode):

$$\cos(10^\circ) \approx 0.9848$$

Substitute this back into the equation:

$$h \approx \frac{6370 \text{ km}}{0.9848} - 6370 \text{ km}$$

$$h \approx 6468.27 \text{ km} - 6370 \text{ km}$$

$$h \approx 98.27 \text{ km}$$

*(Note: Interestingly, this is incredibly close to the modern definition of the edge of space, the Kármán line, which is at 100 km!)*

---

### Final Answer
1. The solar depression angle $\phi$ implied by the measured time is **$10^\circ$**.
2. The estimated atmospheric height $h$ is approximately **98.27 km**.