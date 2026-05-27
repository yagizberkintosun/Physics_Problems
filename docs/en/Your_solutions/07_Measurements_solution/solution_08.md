## 8. Mass-Spring Measurements (Manual Calculations)

### 1. Experimental Data (Sample Run)
Assuming a precise suspended mass of $m = 1.00\text{ kg}$ (zero uncertainty). Using the simulator's timing function to measure the time for 10 complete oscillations ($t_{10}$), we gathered the following 10 trials. The period ($T$) for a single oscillation is calculated as $T = t_{10} / 10$.

| Trial | Time for 10 Osc ($t_{10}$ in s) | Period ($T$ in s) |
|-------|---------------------------------|-------------------|
| 1     | 10.04                           | 1.004             |
| 2     | 9.96                            | 0.996             |
| 3     | 10.02                           | 1.002             |
| 4     | 9.98                            | 0.998             |
| 5     | 10.05                           | 1.005             |
| 6     | 9.95                            | 0.995             |
| 7     | 10.01                           | 1.001             |
| 8     | 9.99                            | 0.999             |
| 9     | 10.06                           | 1.006             |
| 10    | 9.94                            | 0.994             |

---

### 2. Calculating Mean Period ($\bar{T}$) and Standard Deviation ($\sigma_T$)

**Mean Period:**
$$\bar{T} = \frac{1}{10} \sum_{i=1}^{10} T_i = \frac{10.000}{10} = 1.000\text{ s}$$

**Standard Deviation ($\sigma_T$):**
Using the sample standard deviation formula: $\sigma_T = \sqrt{\frac{\sum (T_i - \bar{T})^2}{N-1}}$
$$\sigma_T \approx 0.00427\text{ s}$$

**Uncertainty of the Mean ($\Delta T$):**
The uncertainty of a mean value derived from multiple trials is calculated using the Standard Error of the Mean:
$$\Delta T = \frac{\sigma_T}{\sqrt{N}} = \frac{0.00427}{\sqrt{10}} \approx 0.00135\text{ s}$$

*Reported Period:* $T = (1.0000 \pm 0.0014)\text{ s}$

---

### 3. Calculating the Spring Constant ($k$)
The period of a mass-spring system is given by:
$$T = 2\pi\sqrt{\frac{m}{k}}$$

Rearranging to solve for the spring constant $k$:
$$k = \frac{4\pi^2 m}{\bar{T}^2}$$
$$k = \frac{4\pi^2 (1.00\text{ kg})}{(1.000\text{ s})^2} = 4\pi^2 \approx 39.478\text{ N/m}$$

---

### 4. Measurement Uncertainty of $k$ ($\Delta k$)
To find the measurement uncertainty in the spring constant, we propagate the error from our period measurement. Because the mass $m$ has "zero uncertainty" ($\Delta m = 0$), all the experimental error comes from the period $T$. 

Using the power rule for relative uncertainty (since $T$ is squared in the denominator):
$$\frac{\Delta k}{k} = 2 \left( \frac{\Delta T}{\bar{T}} \right)$$

Solving for the absolute uncertainty ($\Delta k$):
$$\Delta k = k \cdot 2 \cdot \left( \frac{\Delta T}{\bar{T}} \right)$$
$$\Delta k = 39.478 \cdot 2 \cdot \left( \frac{0.00135}{1.000} \right) = 39.478 \cdot 0.0027 \approx 0.1066\text{ N/m}$$

---

### Final Result
Rounding to the correct significant figures (standard convention dictates absolute uncertainty is rounded to one significant figure, and the nominal value matches its decimal place):
* $\Delta k \approx 0.1\text{ N/m}$
* $k \approx 39.5\text{ N/m}$

**Calculated Spring Constant:**
$$k = (39.5 \pm 0.1)\text{ N/m}$$