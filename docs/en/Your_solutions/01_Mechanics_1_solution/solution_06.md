# Variable Velocity: Kinematics Analysis

This document calculates the position and acceleration of an object given its velocity as a function of time and its initial position.

---

## 1. Given Parameters
* **Velocity Function:** $v(t) = t^2 + 2t - 5$
* **Initial Condition:** At $t = 0$, position $x = 4$
* **Target Time:** $t = 3$

---

## 2. Calculating Acceleration ($a$)
Acceleration is the first derivative of velocity with respect to time:

$$a(t) = \frac{dv}{dt}$$
$$a(t) = \frac{d}{dt}(t^2 + 2t - 5)$$
$$a(t) = 2t + 2$$

**Acceleration at $t = 3$:**
$$a(3) = 2(3) + 2 = 8 \text{ units/s}^2$$

---

## 3. Calculating Position ($x$)
Position is the integral of velocity with respect to time:

$$x(t) = \int v(t) \, dt$$
$$x(t) = \int (t^2 + 2t - 5) \, dt$$
$$x(t) = \frac{1}{3}t^3 + t^2 - 5t + C$$

### Solving for $C$:
Using the initial condition $x(0) = 4$:
$$4 = \frac{1}{3}(0)^3 + (0)^2 - 5(0) + C \implies C = 4$$

**The position function is:**
$$x(t) = \frac{1}{3}t^3 + t^2 - 5t + 4$$

**Position at $t = 3$:**
$$x(3) = \frac{1}{3}(3)^3 + (3)^2 - 5(3) + 4$$
$$x(3) = 9 + 9 - 15 + 4$$
$$x(3) = 7 \text{ units}$$

---

## Summary of Results at $t = 3$

| Parameter | Function | Value at $t = 3$ |
| :--- | :--- | :--- |
| **Velocity** | $v(t) = t^2 + 2t - 5$ | $10 \text{ units/s}$ |
| **Acceleration** | $a(t) = 2t + 2$ | $8 \text{ units/s}^2$ |
| **Position** | $x(t) = \frac{1}{3}t^3 + t^2 - 5t + 4$ | $7 \text{ units}$ |