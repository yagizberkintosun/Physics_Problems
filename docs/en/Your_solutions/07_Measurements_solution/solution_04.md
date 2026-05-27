## 4. Relative Uncertainty

### Problem Statement
A car's speedometer has a 5% of uncertainty. If it reads 60 km/h, what is the range of the car's actual speed?

---

### Solution

#### 1. Given Data
* **Measured Speed ($v$):** $60\text{ km/h}$
* **Relative (Percent) Uncertainty:** $5\%$

---

#### 2. Calculating the Absolute Uncertainty ($\Delta v$)
Relative uncertainty describes the error as a fraction (or percentage) of the total measured value. The formula relating relative uncertainty to absolute uncertainty ($\Delta v$) is:
$$\text{Relative Uncertainty} = \frac{\Delta v}{v}$$

To find the absolute uncertainty in the car's speed, we simply calculate $5\%$ of the nominal reading:
$$\Delta v = v \times \left(\frac{5}{100}\right)$$
$$\Delta v = 60\text{ km/h} \times 0.05$$
$$\Delta v = 3\text{ km/h}$$

*Detail Note:* This means the speedometer could be reading up to $3\text{ km/h}$ too fast or $3\text{ km/h}$ too slow.

---

#### 3. Determining the Speed Range
The actual speed of the car falls within a bounded range defined by the measured value minus the absolute uncertainty, and the measured value plus the absolute uncertainty ($v \pm \Delta v$).

* **Minimum possible speed (Lower Bound):** $$v_{\text{min}} = 60\text{ km/h} - 3\text{ km/h} = 57\text{ km/h}$$

* **Maximum possible speed (Upper Bound):** $$v_{\text{max}} = 60\text{ km/h} + 3\text{ km/h} = 63\text{ km/h}$$

### Final Answer
The range of the car's actual speed is **$57\text{ km/h}$ to $63\text{ km/h}$**.

*(This can also be formally written as an interval $[57, 63]\text{ km/h}$ or as $v = 60 \pm 3\text{ km/h}$.)*