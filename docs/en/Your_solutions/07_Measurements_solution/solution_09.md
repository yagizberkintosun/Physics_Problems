## 9. Pendulum Measurements (Manual Calculations)

### 1. Experimental Data (Sample Run)
Assuming a precise string length of $L = 1.00\text{ m}$ (zero uncertainty). Using the manual stopwatch to measure the time for 10 complete oscillations ($t_{10}$), we gathered the following 10 trials. The period ($T$) is calculated as $T = t_{10} / 10$.

| Trial | Time for 10 Osc ($t_{10}$ in s) | Period ($T$ in s) |
|-------|---------------------------------|-------------------|
| 1     | 20.12                           | 2.012             |
| 2     | 19.95                           | 1.995             |
| 3     | 20.08                           | 2.008             |
| 4     | 20.21                           | 2.021             |
| 5     | 19.88                           | 1.988             |
| 6     | 20.01                           | 2.001             |
| 7     | 20.15                           | 2.015             |
| 8     | 19.92                           | 1.992             |
| 9     | 20.05                           | 2.005             |
| 10    | 20.18                           | 2.018             |

---

### 2. Calculating Mean Period ($\bar{T}$) and Standard Deviation ($\sigma_T$)

**Mean Period:**
$$\bar{T} = \frac{1}{10} \sum_{i=1}^{10} T_i = \frac{20.055}{10} = 2.0055\text{ s}$$

**Standard Deviation ($\sigma_T$):**
Using the sample standard deviation formula: $\sigma_T = \sqrt{\frac{\sum (T_i - \bar{T})^2}{N-1}}$
$$\sigma_T \approx 0.011\text{ s}$$

**Uncertainty of the Mean ($\Delta T$):**
In physics, the uncertainty of a mean value from multiple trials is given by the Standard Error:
$$\Delta T = \frac{\sigma_T}{\sqrt{N}} = \frac{0.011}{\sqrt{10}} \approx 0.0035\text{ s}$$

*Reported Period:* $T = (2.0055 \pm 0.0035)\text{ s}$

---

### 3. Calculating Acceleration Due to Gravity ($g$)
The period of a simple pendulum is given by:
$$T = 2\pi\sqrt{\frac{L}{g}}$$

Rearranging to solve for $g$:
$$g = \frac{4\pi^2 L}{\bar{T}^2}$$
$$g = \frac{4\pi^2 (1.00\text{ m})}{(2.0055\text{ s})^2} = \frac{39.478}{4.022} \approx 9.815\text{ m/s}^2$$

---

### 4. Measurement Uncertainty of $g$ ($\Delta g$)
To find the uncertainty in gravity, we propagate the error from our period measurement. Because $L$ has "zero uncertainty" (as stated in the prompt, $\Delta L = 0$), all error comes from $T$. 

Using the power rule for relative uncertainty (since $T$ is squared in the denominator):
$$\frac{\Delta g}{g} = 2 \left( \frac{\Delta T}{\bar{T}} \right)$$

Solving for absolute uncertainty ($\Delta g$):
$$\Delta g = g \cdot 2 \cdot \left( \frac{\Delta T}{\bar{T}} \right)$$
$$\Delta g = 9.815 \cdot 2 \cdot \left( \frac{0.0035}{2.0055} \right) = 9.815 \cdot 0.00349 \approx 0.034\text{ m/s}^2$$

---

### Final Result
Rounding to the correct significant figures (uncertainty to 1 sig fig, value matched to decimal place):
* $\Delta g \approx 0.03\text{ m/s}^2$
* $g \approx 9.81\text{ m/s}^2$

**Calculated Gravity:**
$$g = (9.81 \pm 0.03)\text{ m/s}^2$$

*(Note for Part 2: If performing the physical real-life experiment, swap out the sample data table above with your own cellphone stopwatch measurements, and re-run the mean/standard deviation calculations using the same formulas!)*