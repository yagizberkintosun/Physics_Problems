# Physics Problem: Transformer Voltage and Current

## 1. Problem Statement
We are analyzing a transformer with the following specifications:
*   **Primary Turns ($N_p$):** 1000 turns
*   **Secondary Turns ($N_s$):** 200 turns
*   **Primary Voltage ($V_p$):** 120 V (AC)
*   **Secondary Current ($I_s$):** 3 A

**Goal:** Calculate the secondary voltage ($V_s$) and the current in the primary coil ($I_p$).

---

## 2. Fundamental Physics Principles

### The Transformer Equation
The ratio of the secondary voltage to the primary voltage is equal to the ratio of the number of turns in the secondary coil to the number of turns in the primary coil:
$$\frac{V_s}{V_p} = \frac{N_s}{N_p}$$

### Conservation of Energy (Ideal Transformer)
Assuming an ideal transformer (100% efficiency), the power in the primary coil equals the power in the secondary coil ($P_p = P_s$). Since $P = VI$, we can derive the relationship for current:
$$V_p \cdot I_p = V_s \cdot I_s \implies \frac{I_p}{I_s} = \frac{V_s}{V_p} = \frac{N_s}{N_p}$$
*Note: This shows that current is inversely proportional to the number of turns.*

---

## 3. Step-by-Step Calculation

### Step A: Calculate Secondary Voltage ($V_s$)
Using the transformer equation:
$$V_s = V_p \cdot \left( \frac{N_s}{N_p} \right)$$
$$V_s = 120\ \text{V} \cdot \left( \frac{200}{1000} \right)$$
$$V_s = 120\ \text{V} \cdot 0.2$$
**$V_s = 24\ \text{V}$**

### Step B: Calculate Primary Current ($I_p$)
Using the inverse turns ratio for current:
$$I_p = I_s \cdot \left( \frac{N_s}{N_p} \right)$$
$$I_p = 3\ \text{A} \cdot \left( \frac{200}{1000} \right)$$
$$I_p = 3\ \text{A} \cdot 0.2$$
**$I_p = 0.6\ \text{A}$**

---

## 4. Final Results Summary

| Parameter | Value |
| :--- | :--- |
| **Secondary Voltage ($V_s$)** | **24 V** |
| **Primary Current ($I_p$)** | **0.6 A** |

**Teacher's Note:** This is a **step-down transformer** because the number of turns decreases from primary to secondary ($1000 \to 200$), which causes the voltage to decrease ($120\ \text{V} \to 24\ \text{V}$). To conserve energy, as the voltage steps down, the current must "step up" in the secondary. This is why the primary current ($0.6\ \text{A}$) is significantly lower than the secondary current ($3\ \text{A}$).