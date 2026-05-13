# Physics Problem: Capacitors in Parallel

## 1. Problem Statement
We have the following scenario:
*   Two capacitors: $C_1 = 4\ \mu\text{F}$ and $C_2 = 6\ \mu\text{F}$.
*   Connection: **Parallel**.
*   Voltage Source ($V$): 10 V battery.

**Goal:** Calculate the **total charge stored** ($Q_{total}$) and the **total energy stored** ($U_{total}$) in the system.

---

## 2. Fundamental Physics Concepts

### Capacitors in Parallel
When capacitors are connected in parallel, the potential difference (voltage) across each capacitor is identical to the battery voltage. The total equivalent capacitance ($C_{eq}$) is the sum of the individual capacitances:
$$C_{eq} = C_1 + C_2 + \dots + C_n$$

### Capacitance, Charge, and Voltage
The relationship between charge ($Q$), capacitance ($C$), and voltage ($V$) is:
$$Q = C \cdot V$$

### Energy Stored in a Capacitor
The electrical potential energy ($U$) stored in a capacitor can be calculated using:
$$U = \frac{1}{2} C V^2$$

---

## 3. Step-by-Step Calculation

### Step A: Find the Equivalent Capacitance
Since the capacitors are in parallel, we add their values directly:
$$C_{eq} = C_1 + C_2$$
$$C_{eq} = 4\ \mu\text{F} + 6\ \mu\text{F}$$
**$C_{eq} = 10\ \mu\text{F}$** (or $10 \times 10^{-6}\ \text{F}$)

### Step B: Calculate Total Charge Stored
Using the total equivalent capacitance and the battery voltage:
$$Q_{total} = C_{eq} \cdot V$$
$$Q_{total} = (10 \times 10^{-6}\ \text{F}) \cdot 10\ \text{V}$$
$$Q_{total} = 100 \times 10^{-6}\ \text{C}$$
**$Q_{total} = 100\ \mu\text{C}$**

### Step C: Calculate Total Energy Stored
Using the energy formula for the entire system:
$$U_{total} = \frac{1}{2} C_{eq} V^2$$
$$U_{total} = \frac{1}{2} \cdot (10 \times 10^{-6}\ \text{F}) \cdot (10\ \text{V})^2$$
$$U_{total} = (5 \times 10^{-6}\ \text{F}) \cdot 100\ \text{V}^2$$
$$U_{total} = 500 \times 10^{-6}\ \text{J}$$
**$U_{total} = 5 \times 10^{-4}\ \text{J}$** (or 0.5 mJ)

---

## 4. Final Results Summary

| Parameter | Value |
| :--- | :--- |
| **Equivalent Capacitance ($C_{eq}$)** | $10\ \mu\text{F}$ |
| **Total Charge ($Q_{total}$)** | $100\ \mu\text{C}$ |
| **Total Energy ($U_{total}$)** | $0.5\ \text{mJ}$ |

**Explanation for the Teacher:** In a parallel circuit, the total capacitance increases because the "plates" of the capacitors effectively become larger, allowing more charge to be stored at the same voltage. This is why $C_{eq}$ is higher than the individual components, leading to a total charge of $100\ \mu\text{C}$ and a stored energy of 0.5 mJ.