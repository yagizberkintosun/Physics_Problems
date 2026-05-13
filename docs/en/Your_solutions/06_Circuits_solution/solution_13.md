# Physics Problem: Transformer Turns Ratio

## 1. Problem Statement
We are analyzing a step-down transformer with the following parameters:
*   **Primary Voltage ($V_p$):** 120 V AC
*   **Secondary Voltage ($V_s$):** 9.0 V AC
*   **Primary Coil Turns ($N_p$):** 400 turns

**Goal:** Determine the required number of turns for the **secondary coil** ($N_s$).

---

## 2. Fundamental Physics Principles

### The Transformer Equation
The primary and secondary coils of a transformer are linked by the magnetic flux in the core. According to Faraday's Law of Induction, the ratio of the voltages is directly proportional to the ratio of the number of turns in each coil:

$$\frac{V_s}{V_p} = \frac{N_s}{N_p}$$

This relationship allows us to calculate an unknown number of turns if the voltage ratio and the other coil's turns are known.

---

## 3. Step-by-Step Calculation

### Step A: Isolate the Unknown Variable
We need to find $N_s$. We rearrange the transformer equation to solve for the secondary turns:
$$N_s = N_p \cdot \left( \frac{V_s}{V_p} \right)$$

### Step B: Substitute the Given Values
Plug the values from **image_1c49db.png** into the rearranged formula:
$$N_s = 400 \cdot \left( \frac{9.0\ \text{V}}{120\ \text{V}} \right)$$

### Step C: Solve the Arithmetic
1. Calculate the voltage ratio (the "step-down" factor):
   $$\frac{9}{120} = 0.075$$
2. Multiply by the primary turns:
   $$N_s = 400 \times 0.075$$
   $$N_s = 30$$

---

## 4. Final Result
The secondary coil must have:
**$$N_s = 30\ \text{turns}$$**

**Explanation for the Teacher:** Since the output voltage ($9\ \text{V}$) is much lower than the input voltage ($120\ \text{V}$), this is a **step-down transformer**. Specifically, the voltage is reduced by a factor of 13.33. Therefore, the number of turns in the secondary coil must also be 13.33 times smaller than the primary coil ($400 / 13.33 \approx 30$).