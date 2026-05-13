# Physics Problem: Kirchhoff's Laws in a Multi-Loop Circuit

## 1. Problem Statement
We are analyzing a two-loop circuit with the following components:
*   **Left Branch:** Resistor $R_1 = 20\ \Omega$, Battery $\mathcal{E}_1 = 4.5\ \text{V}$, and Internal Resistance $r_{w1} = 1\ \Omega$.
*   **Right Branch:** Battery $\mathcal{E}_2 = 9\ \text{V}$ and Internal Resistance $r_{w2} = 1\ \Omega$.
*   **Shared (Middle) Branch:** Resistor $R_2 = 10\ \Omega$.

**Goal:** Calculate the currents $I_1$, $I_2$, and $I_3$ flowing through the left, middle, and right branches respectively.

---

## 2. Fundamental Physics Laws

### Kirchhoff’s Junction Rule (KCL)
The sum of currents entering a junction must equal the sum of currents leaving it (Conservation of Charge).
$$\sum I_{in} = \sum I_{out}$$

### Kirchhoff’s Loop Rule (KVL)
The sum of potential differences around any closed loop must be zero (Conservation of Energy).
$$\sum \Delta V = 0$$

---

## 3. Circuit Setup and Definitions

We define the directions of the currents as follows:
1.  **$I_1$**: Flows **upward** through the left branch (clockwise in the left loop).
2.  **$I_3$**: Flows **upward** through the right branch (counter-clockwise in the right loop).
3.  **$I_2$**: Flows **downward** through the shared middle resistor ($R_2$).

### Step A: The Junction Equation
At the top junction node:
$$I_1 + I_3 = I_2 \quad \text{--- (Equation 1)}$$

---

## 4. Applying the Loop Rule (KVL)

### Loop 1: Left Loop (Clockwise)
Starting from the bottom-left corner and moving clockwise:
1.  Pass through $\mathcal{E}_1$: $+4.5\ \text{V}$ (moving from - to +)
2.  Pass through $r_{w1}$: $-I_1 \cdot 1\ \Omega$ (drop)
3.  Pass through $R_1$: $-I_1 \cdot 20\ \Omega$ (drop)
4.  Pass through $R_2$: $-I_2 \cdot 10\ \Omega$ (drop)

**Equation:**
$$4.5 - I_1(1) - I_1(20) - I_2(10) = 0$$
$$4.5 - 21I_1 - 10I_2 = 0 \quad \text{--- (Equation 2)}$$

### Loop 2: Right Loop (Counter-Clockwise)
Starting from the bottom-right and moving counter-clockwise:
1.  Pass through $\mathcal{E}_2$: $+9\ \text{V}$
2.  Pass through $r_{w2}$: $-I_3 \cdot 1\ \Omega$ (drop)
3.  Pass through $R_2$: $-I_2 \cdot 10\ \Omega$ (drop)

**Equation:**
$$9 - I_3(1) - 10I_2 = 0 \quad \text{--- (Equation 3)}$$

---

## 5. Solving the System of Equations

We have three unknowns ($I_1, I_2, I_3$) and three equations.

**1. Isolate $I_3$ using Equation 1:**
$$I_3 = I_2 - I_1$$

**2. Substitute $I_3$ into Equation 3:**
$$9 - (I_2 - I_1) - 10I_2 = 0$$
$$9 - I_2 + I_1 - 10I_2 = 0$$
$$I_1 = 11I_2 - 9 \quad \text{--- (Equation 4)}$$

**3. Substitute Equation 4 into Equation 2:**
$$4.5 - 21(11I_2 - 9) - 10I_2 = 0$$
$$4.5 - 231I_2 + 189 - 10I_2 = 0$$
$$193.5 - 241I_2 = 0$$
$$I_2 = \frac{193.5}{241} \approx \mathbf{0.803\ \text{A}}$$

**4. Find $I_1$ and $I_3$:**
*   $I_1 = 11(0.8029) - 9 \approx \mathbf{-0.168\ \text{A}}$
*   $I_3 = 0.8029 - (-0.1681) \approx \mathbf{0.971\ \text{A}}$

---

## 6. Final Results Summary

| Branch | Current | Direction (based on diagram) |
| :--- | :--- | :--- |
| **Left ($I_1$)** | $-0.168\ \text{A}$ | Downward (Opposite to assumption) |
| **Middle ($I_2$)** | $0.803\ \text{A}$ | Downward |
| **Right ($I_3$)** | $0.971\ \text{A}$ | Upward |

**Note:** The negative sign for $I_1$ indicates that the 9V battery is strong enough to "push" current backward through the 4.5V source, charging it rather than being powered by it.