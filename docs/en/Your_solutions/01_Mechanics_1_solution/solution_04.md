# Vector Calculus: Kinematics Analysis

This document derives the velocity and acceleration vectors for an object whose position is defined by a vector-valued function of time.

---

## 1. Given Position Vector
The position of the object at time $t$ is:
$$\vec{r}(t) = (3t^2)\hat{i} + (5t - 8t^2)\hat{j}$$

---

## 2. Velocity Vector $\vec{v}(t)$
Velocity is the first derivative of the position vector with respect to time:
$$\vec{v}(t) = \frac{d\vec{r}}{dt}$$

We differentiate the $x$ and $y$ components independently:
* **$i$ component:** $\frac{d}{dt}(3t^2) = 6t$
* **$j$ component:** $\frac{d}{dt}(5t - 8t^2) = 5 - 16t$

**Resulting Velocity Vector:**
$$\vec{v}(t) = (6t)\hat{i} + (5 - 16t)\hat{j}$$

---

## 3. Acceleration Vector $\vec{a}(t)$
Acceleration is the derivative of the velocity vector with respect to time:
$$\vec{a}(t) = \frac{d\vec{v}}{dt}$$

Differentiating the velocity components:
* **$i$ component:** $\frac{d}{dt}(6t) = 6$
* **$j$ component:** $\frac{d}{dt}(5 - 16t) = -16$

**Resulting Acceleration Vector:**
$$\vec{a}(t) = 6\hat{i} - 16\hat{j}$$

---

## Summary
| Vector | Equation |
| :--- | :--- |
| **Position** | $\vec{r}(t) = (3t^2)\hat{i} + (5t - 8t^2)\hat{j}$ |
| **Velocity** | $\vec{v}(t) = (6t)\hat{i} + (5 - 16t)\hat{j}$ |
| **Acceleration** | $\vec{a}(t) = 6\hat{i} - 16\hat{j}$ |