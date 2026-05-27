## 2. Propagation of Error II

### Problem Statement
The length and width of a rectangular plate are measured to be $L = (15.3 \pm 0.1)\text{ cm}$ and $W = (8.4 \pm 0.1)\text{ cm}$. Calculate the area of the plate and its uncertainty.

---

### Solution

#### 1. Given Data
* **Length ($L$):** $15.3\text{ cm}$
* **Uncertainty in length ($\Delta L$):** $0.1\text{ cm}$
* **Width ($W$):** $8.4\text{ cm}$
* **Uncertainty in width ($\Delta W$):** $0.1\text{ cm}$

---

#### 2. Calculating the Nominal Area ($A$)
The formula for the area of a rectangle is:
$$A = L \times W$$

Substituting the measured values:
$$A = 15.3\text{ cm} \times 8.4\text{ cm}$$
$$A = 128.52\text{ cm}^2$$

---

#### 3. Calculating the Propagated Uncertainty ($\Delta A$)
When two independent measured variables are multiplied, their uncertainties propagate. In physics and engineering labs, there are two primary ways to compute this depending on whether the errors are treated as **absolute maximum limits (worst-case)** or **independent/random (quadrature)**. 

Both standard approaches are outlined below so you can match your professor's preferred curriculum style:

##### Approach A: Quadrature (Standard Statistical Propagation)
If the measurement errors for length and width are independent and random, we add their relative fractional uncertainties in quadrature:

$$\frac{\Delta A}{A} = \sqrt{\left(\frac{\Delta L}{L}\right)^2 + \left(\frac{\Delta W}{W}\right)^2}$$

1. **Calculate the fractional components:**
   $$\frac{\Delta L}{L} = \frac{0.1}{15.3} \approx 0.006536$$
   $$\frac{\Delta W}{W} = \frac{0.1}{8.4} \approx 0.011905$$

2. **Combine in quadrature:**
   $$\frac{\Delta A}{A} = \sqrt{(0.006536)^2 + (0.011905)^2}$$
   $$\frac{\Delta A}{A} = \sqrt{0.00004272 + 0.00014173} = \sqrt{0.00018445} \approx 0.01358$$

3. **Solve for absolute uncertainty ($\Delta A$):**
   $$\Delta A = 0.01358 \times 128.52\text{ cm}^2 \approx 1.745\text{ cm}^2$$

---

##### Approach B: Upper-Bound / Partial Derivatives Method
If your instructor prefers using absolute maximum limits or the multi-variable calculus approach (partial derivatives):

$$\Delta A = \left| \frac{\partial A}{\partial L} \right| \Delta L + \left| \frac{\partial A}{\partial W} \right| \Delta W$$

1. **Evaluate the partial derivatives:**
   $$\frac{\partial A}{\partial L} = W \quad \text{and} \quad \frac{\partial A}{\partial W} = L$$

2. **Substitute values:**
   $$\Delta A = (W \cdot \Delta L) + (L \cdot \Delta W)$$
   $$\Delta A = (8.4 \times 0.1) + (15.3 \times 0.1)$$
   $$\Delta A = 0.84 + 1.53 = 2.37\text{ cm}^2$$

---

#### 4. Formatting and Significant Figures

* Following standard experimental notation rules, uncertainty values are restricted to **one significant figure** (or rounded up to two if precision demands it). 
* The nominal value decimal position must match the final decimal place of the uncertainty.

* Using **Approach A (Quadrature)**: $\Delta A \approx 2\text{ cm}^2$, meaning $A$ rounds to the nearest whole integer ($129\text{ cm}^2$).
* Using **Approach B (Worst-Case)**: $\Delta A \approx 2\text{ cm}^2$ or $2.4\text{ cm}^2$, matching to either $129\text{ cm}^2$ or $128.5\text{ cm}^2$.

### Final Answer
*(Using standard statistical quadrature error propagation)*
$$A = (129 \pm 2)\text{ cm}^2$$

*(Using the worst-case derivative error propagation)*
$$A = (128.5 \pm 2.4)\text{ cm}^2$$