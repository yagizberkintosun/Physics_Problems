# Physics Problem: Instantaneous Current Calculation

## 1. Problem Statement
We are provided with a time-dependent function for the charge ($Q$) flowing through a wire:
*   **Charge Function:** $Q(t) = 5t^2 + 5$

**Goal:** Calculate the instantaneous current ($I$) at the specific time **$t = 3\ \text{s}$**.

---

## 2. Fundamental Physics Principle

### Definition of Electric Current
Electric current is defined as the rate at which charge flows through a cross-sectional area of a conductor. While average current is $\Delta Q / \Delta t$, the **instantaneous current** is the derivative of the charge function with respect to time:

$$I(t) = \frac{dQ(t)}{dt}$$

This tells us that to find the current at any moment, we must find the slope of the charge-vs-time graph at that exact point.

---

## 3. Step-by-Step Derivation

### Step A: Differentiate the Charge Function
We apply the power rule of differentiation ($\frac{d}{dt} t^n = nt^{n-1}$) to our function $Q(t) = 5t^2 + 5$:

1.  Take the derivative of the first term: $\frac{d}{dt}(5t^2) = 10t$
2.  Take the derivative of the constant term: $\frac{d}{dt}(5) = 0$

Combining these, we get the general equation for current in this wire:
**$$I(t) = 10t$$**

### Step B: Evaluate at the Given Time
Now, we substitute the specific time value ($t = 3\ \text{s}$) into our new current equation:
$$I(3) = 10(3)$$
$$I(3) = 30$$

---

## 4. Final Result
The instantaneous current flowing through the wire at $t = 3\ \text{s}$ is:
**$$I = 30\ \text{A}$$**

**Explanation for the Teacher:** Since the charge function $Q(t)$ is quadratic, the current $I(t)$ is linear. This indicates that the current is not constant but is increasing at a steady rate of $10\ \text{A/s}$ (constant acceleration of charge). At the 3-second mark, that rate has reached exactly 30 Amperes.