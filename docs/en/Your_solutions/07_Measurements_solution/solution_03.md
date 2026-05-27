
## 1. Propagation of Error I

### Problem Statement
The radius of a sphere is measured to be $r = (6.20 \pm 0.05)\text{ cm}$. Calculate the volume of the sphere and its associated uncertainty.

---

### Solution

#### 1. Given Data
* **Measured radius ($r$):** $6.20\text{ cm}$
* **Uncertainty in radius ($\Delta r$):** $0.05\text{ cm}$

#### 2. Calculating the Nominal Volume ($V$)
The formula for the volume of a sphere is:
$$V = \frac{4}{3}\pi r^3$$

Substituting the nominal value of $r$:
$$V = \frac{4}{3} \cdot \pi \cdot (6.20\text{ cm})^3$$
$$V \approx 997.974\text{ cm}^3$$

#### 3. Calculating the Propagated Uncertainty ($\Delta V$)
To find the uncertainty in the volume, we use the derivative-based approach for error propagation. The general formula for a single variable function $V(r)$ is:
$$\Delta V = \left| \frac{dV}{dr} \right| \cdot \Delta r$$

1. **Find the derivative of $V$ with respect to $r$** (which represents the surface area):
   $$\frac{dV}{dr} = 4\pi r^2$$

2. **Substitute the known values into the uncertainty equation:**
   $$\Delta V = (4\pi r^2) \cdot \Delta r$$
   $$\Delta V = 4 \cdot \pi \cdot (6.20\text{ cm})^2 \cdot 0.05\text{ cm}$$
   $$\Delta V \approx 24.152\text{ cm}^3$$

> **Alternative Method (Fractional Uncertainties):**
> Because $V \propto r^3$, the relative (fractional) uncertainty can also be calculated as:
> $$\frac{\Delta V}{V} = 3 \cdot \frac{\Delta r}{r} \implies \Delta V = 3 \cdot \frac{0.05}{6.20} \cdot 997.974 \approx 24.145\text{ cm}^3$$

#### 4. Formatting and Significant Figures
Standard experimental physics convention dictates rounding the uncertainty to **one significant figure** (or two, if the leading digit is a 1). Here, $\Delta V \approx 20\text{ cm}^3$. The decimal place of the nominal volume must match this precision, so we round to the nearest tens place.

### Final Answer
$$V = (1000 \pm 20)\text{ cm}^3$$
*(Or in scientific notation to clarify precision: $V = (1.00 \pm 0.02) \times 10^3\text{ cm}^3$)*

<br>

---

## 2. Propagation of Error II

### Problem Statement
The length and width of a rectangular plate are measured to be $L = (15.3 \pm 0.1)\text{ cm}$ and $W = (8.4 \pm 0.1)\text{ cm}$. Calculate the area of the plate and its uncertainty.

---

### Solution

#### 1. Given Data
* **Length ($L$):** $15.3\text{ cm} \quad (\Delta L = 0.1\text{ cm})$
* **Width ($W$):** $8.4\text{ cm} \quad (\Delta W = 0.1\text{ cm})$

#### 2. Calculating the Nominal Area ($A$)
$$A = L \times W = 15.3\text{ cm} \times 8.4\text{ cm} = 128.52\text{ cm}^2$$

#### 3. Calculating the Propagated Uncertainty ($\Delta A$)
When multiplying independent variables, uncertainties can be calculated using either **standard statistical propagation (quadrature)** or the **absolute maximum limits** method. Both are provided below based on standard lab practices.

**Approach A: Quadrature (Random/Independent Errors)**
Add the relative fractional uncertainties in quadrature:
$$\frac{\Delta A}{A} = \sqrt{\left(\frac{\Delta L}{L}\right)^2 + \left(\frac{\Delta W}{W}\right)^2}$$
$$\frac{\Delta A}{A} = \sqrt{\left(\frac{0.1}{15.3}\right)^2 + \left(\frac{0.1}{8.4}\right)^2} \approx \sqrt{0.0000427 + 0.0001417} \approx 0.01358$$
$$\Delta A = 0.01358 \times 128.52\text{ cm}^2 \approx 1.745\text{ cm}^2$$

**Approach B: Partial Derivatives (Worst-Case Upper Bound)**
$$\Delta A = \left| \frac{\partial A}{\partial L} \right| \Delta L + \left| \frac{\partial A}{\partial W} \right| \Delta W = W\Delta L + L\Delta W$$
$$\Delta A = (8.4 \times 0.1) + (15.3 \times 0.1) = 0.84 + 1.53 = 2.37\text{ cm}^2$$

#### 4. Formatting and Significant Figures
Matching the nominal value to the single-sig-fig uncertainty:
* **Quadrature:** $\Delta A \approx 2\text{ cm}^2 \implies A \approx 129\text{ cm}^2$
* **Worst-Case:** $\Delta A \approx 2\text{ cm}^2$ or $2.4\text{ cm}^2 \implies A \approx 129\text{ cm}^2$ or $128.5\text{ cm}^2$

### Final Answer
*(Using standard statistical quadrature)*
$$A = (129 \pm 2)\text{ cm}^2$$

<br>

---

## 3. Propagation of Error III

### Problem Statement
The resistance $R$ is calculated using Ohm's Law, $R = V / I$. If the voltage is measured as $V = (10.0 \pm 0.2)\text{ V}$ and the current as $I = (2.00 \pm 0.05)\text{ A}$, what is the calculated resistance and its uncertainty?

---

### Solution

#### 1. Given Data
* **Voltage ($V$):** $10.0\text{ V} \quad (\Delta V = 0.2\text{ V})$
* **Current ($I$):** $2.00\text{ A} \quad (\Delta I = 0.05\text{ A})$

#### 2. Calculating the Nominal Resistance ($R$)
Using Ohm's Law:
$$R = \frac{V}{I} = \frac{10.0\text{ V}}{2.00\text{ A}} = 5.00\ \Omega$$

#### 3. Calculating the Propagated Uncertainty ($\Delta R$)
Division follows the same relative error propagation rules as multiplication.

**Approach A: Quadrature (Standard Statistical Propagation)**
$$\frac{\Delta R}{R} = \sqrt{\left(\frac{\Delta V}{V}\right)^2 + \left(\frac{\Delta I}{I}\right)^2}$$
$$\frac{\Delta R}{R} = \sqrt{\left(\frac{0.2}{10.0}\right)^2 + \left(\frac{0.05}{2.00}\right)^2} = \sqrt{(0.02)^2 + (0.025)^2}$$
$$\frac{\Delta R}{R} = \sqrt{0.0004 + 0.000625} = \sqrt{0.001025} \approx 0.032015$$
$$\Delta R = 0.032015 \times 5.00\ \Omega \approx 0.1601\ \Omega$$

**Approach B: Partial Derivatives (Absolute Worst-Case Method)**
$$\Delta R = \left| \frac{\partial R}{\partial V} \right| \Delta V + \left| \frac{\partial R}{\partial I} \right| \Delta I$$
$$\Delta R = \left(\frac{1}{I}\right)\Delta V + \left(\frac{V}{I^2}\right)\Delta I$$
$$\Delta R = \left(\frac{1}{2.00}\right)(0.2) + \left(\frac{10.0}{(2.00)^2}\right)(0.05)$$
$$\Delta R = 0.10 + 2.5(0.05) = 0.10 + 0.125 = 0.225\ \Omega$$

#### 4. Formatting and Significant Figures
Rounding the absolute uncertainty properly (keeping the leading "1" in the quadrature method for extra precision, and matching decimal places):
* **Quadrature:** $\Delta R \approx 0.16\ \Omega \implies R \approx 5.00\ \Omega$
* **Worst-Case:** $\Delta R \approx 0.2\ \Omega \implies R \approx 5.0\ \Omega$

### Final Answer
*(Using standard statistical quadrature)*
$$R = (5.00 \pm 0.16)\ \Omega$$

*(Using the absolute upper-bound method)*
$$R = (5.0 \pm 0.2)\ \Omega$$