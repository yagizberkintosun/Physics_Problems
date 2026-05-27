## 1. Propagation of Error I

### Problem Statement
The radius of a sphere is measured to be $r = (6.20 \pm 0.05)\text{ cm}$. Calculate the volume of the sphere and its associated uncertainty.

---

### Solution

#### 1. Given Data
* **Measured radius ($r$):** $6.20\text{ cm}$
* **Uncertainty in radius ($\Delta r$):** $0.05\text{ cm}$

---

#### 2. Calculating the Nominal Volume ($V$)
The formula for the volume of a sphere is:
$$V = \frac{4}{3}\pi r^3$$

Substituting the nominal value of $r$:
$$V = \frac{4}{3} \cdot \pi \cdot (6.20\text{ cm})^3$$
$$V = \frac{4}{3} \cdot \pi \cdot 238.328\text{ cm}^3$$
$$V \approx 997.974\text{ cm}^3$$

---

#### 3. Calculating the Propagated Uncertainty ($\Delta V$)
To find the uncertainty in the volume, we use the derivative-based approach for error propagation. 

The general formula for the propagation of uncertainty for a single variable function $V(r)$ is:
$$\Delta V = \left| \frac{dV}{dr} \right| \cdot \Delta r$$

1. **Find the derivative of $V$ with respect to $r$:**
   $$\frac{dV}{dr} = \frac{4}{3}\pi \cdot (3r^2) = 4\pi r^2$$
   *(Note: This derivative is geometrically equal to the surface area of the sphere).*

2. **Substitute the known values into the uncertainty equation:**
   $$\Delta V = (4\pi r^2) \cdot \Delta r$$
   $$\Delta V = 4 \cdot \pi \cdot (6.20\text{ cm})^2 \cdot 0.05\text{ cm}$$
   $$\Delta V = 4 \cdot \pi \cdot 38.44\text{ cm}^2 \cdot 0.05\text{ cm}$$
   $$\Delta V = 7.688\pi\text{ cm}^3$$
   $$\Delta V \approx 24.152\text{ cm}^3$$

> **Alternative Method (Fractional Uncertainties):**
> Because $V \propto r^3$, the relative (fractional) uncertainty can also be calculated as:
> $$\frac{\Delta V}{V} = 3 \cdot \frac{\Delta r}{r}$$
> $$\Delta V = 3 \cdot \frac{0.05}{6.20} \cdot 997.974 \approx 24.145\text{ cm}^3$$
> *Both methods yield equivalent results depending on intermediate rounding choices.*

---

#### 4. Formatting and Significant Figures
* **Uncertainty Rounding:** Standard experimental physics convention states that experimental uncertainty should generally be rounded to **one significant figure** (or two, if the leading digit is a 1). Here, $\Delta V \approx 24\text{ cm}^3$.
* **Value Matching:** The decimal place of the nominal value must match the precision of the uncertainty. Therefore, we round the volume to the nearest integer.

* $V \approx 1000\text{ cm}^3$ (or $1.00 \times 10^3\text{ cm}^3$ to maintain precision clarity)
* $\Delta V \approx 20\text{ cm}^3$ (or $0.02 \times 10^3\text{ cm}^3$)

### Final Answer
The volume of the sphere and its associated uncertainty is:
$$V = (1.00 \pm 0.02) \times 10^3\text{ cm}^3$$

*(Alternatively, without scientific notation: $V = 1000 \pm 20\text{ cm}^3$)*