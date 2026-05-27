## 6. Instrument Precision

### Problem Statement
A digital thermometer reads 25.4°C. Assuming the uncertainty is half the value of the last digit, what is the absolute uncertainty of this measurement?

---

### Solution

#### 1. Given Data
* **Measured Temperature ($T$):** 25.4°C
* **Uncertainty Rule:** Half the value of the last digit.

---

#### 2. Determining the Resolution
To find the value of the "last digit," we look at the decimal places in the provided measurement (25.4°C). 
* The last digit ('4') is in the tenths place. 
* This means the smallest discrete step the thermometer displays (its resolution or least count) is **0.1°C**.

---

#### 3. Calculating the Absolute Uncertainty ($\Delta T$)
Following the explicit instruction in the problem, the absolute uncertainty is half of that smallest resolution value.

$$\Delta T = \frac{0.1\text{°C}}{2} = 0.05\text{°C}$$

> **Important Detail for Lab Context:** > * In standard experimental physics, the rule of "half the smallest division" is typically reserved for **analog** instruments (like a mercury thermometer where you can visually estimate between lines). 
> * For **digital** instruments, the standard convention is usually to take the full resolution ($\pm 0.1\text{°C}$) because you cannot know if internal rounding occurred (e.g., a true 25.44°C and 25.36°C might both display as 25.4°C). 
> * *However*, since this specific problem explicitly dictates using "half the value of the last digit," you must follow the prompt's constraint to arrive at 0.05°C. Noting this distinction shows excellent experimental awareness!

---

#### 4. Formatting the Final Value
If you need to report the full measurement with its uncertainty, remember that the decimal places must align. Because our calculated uncertainty (0.05°C) has two decimal places, we add a placeholder zero to the original reading to match the precision.

### Final Answer
The absolute uncertainty of this measurement is **0.05°C**.

*(If written as a complete formal measurement: $T = 25.40 \pm 0.05$°C)*