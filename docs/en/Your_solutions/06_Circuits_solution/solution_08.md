# Physics Problem: AC Voltage Equation

## 1. Problem Statement
We are given:
*   The equation for alternating current (AC): $I(t) = 2 \sin(120\pi t)$
*   A single resistor with resistance: $R = 50\ \Omega$

**Goal:** Determine the mathematical equation for the instantaneous voltage $V(t)$ across the resistor.

---

## 2. Fundamental Physics Concepts

### Ohm's Law in AC Circuits
In a purely resistive circuit, Ohm's Law holds true for instantaneous values. This means the voltage at any specific moment is directly proportional to the current at that same moment:
$$V(t) = I(t) \cdot R$$

### Phase Relationship
In a circuit containing only resistance, the current and voltage are **in phase**. This means they reach their peak values and zero points at the exact same time. Consequently, the functional form (the sine wave) remains identical; only the amplitude changes.

---

## 3. Step-by-Step Derivation

### Step A: Identify Components of the Current Equation
The general form of an AC current equation is $I(t) = I_{peak} \sin(\omega t)$. From the given equation $I(t) = 2 \sin(120\pi t)$, we can identify:
*   **Peak Current ($I_{peak}$):** $2\ \text{A}$
*   **Angular Frequency ($\omega$):** $120\pi\ \text{rad/s}$

### Step B: Apply Ohm's Law
To find the voltage equation, we multiply the entire current function by the resistance:
$$V(t) = [2 \sin(120\pi t)] \times 50\ \Omega$$

### Step C: Simplify the Expression
Multiply the peak current by the resistance to find the peak voltage ($V_{peak}$):
$$V(t) = (2 \times 50) \sin(120\pi t)$$
$$V(t) = 100 \sin(120\pi t)$$

---

## 4. Final Result
The equation for the voltage across the resistor in **image_1cb23e.png** is:
**$$V(t) = 100 \sin(120\pi t)$$**

### Summary of Parameters:
| Parameter | Value |
| :--- | :--- |
| **Peak Voltage ($V_{peak}$)** | $100\ \text{V}$ |
| **Angular Frequency ($\omega$)** | $120\pi\ \text{rad/s}$ |
| **Frequency ($f$)** | $60\ \text{Hz}$ |

**Teacher's Note:** Because the load is purely resistive, there is no phase shift ($\phi = 0$). The voltage "follows" the current perfectly, resulting in a peak voltage of 100 V when the current hits its 2 A peak.