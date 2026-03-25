# Elimination of Time and Interpretation of Acceleration

This document analyzes a particle's trajectory defined by parametric equations, eliminates the time parameter to find the Cartesian path, and derives velocity and acceleration vectors.

---

## 1. Given Parametric Equations
The path of the object is given by:
* $x(t) = 2t^2$
* $y(t) = 3t^3$

---

## 2. Eliminating the Parameter $t$
To find the equation of the trajectory in terms of $x$ and $y$:

1.  From the $x$ equation, solve for $t$:
    $$x = 2t^2 \implies t^2 = \frac{x}{2} \implies t = \left(\frac{x}{2}\right)^{1/2}$$

2.  Substitute $t$ into the $y$ equation:
    $$y = 3t^3 = 3\left[\left(\frac{x}{2}\right)^{1/2}\right]^3$$
    $$y = 3\left(\frac{x}{2}\right)^{3/2}$$

**Resulting Cartesian Path:**
$$y = \frac{3}{2\sqrt{2}}x^{3/2}$$
This curve is known as a **semi-cubical parabola**.

---

## 3. Trajectory Description
The trajectory starts at the origin $(0,0)$ at $t=0$. As $t$ increases, both $x$ and $y$ increase. Since $y \propto x^{1.5}$, the curve bends upward more sharply than a standard parabola ($y \propto x^2$).

---

## 4. Velocity and Acceleration Vectors

### Velocity $\vec{v}(t)$
$$\vec{v}(t) = \left\langle \frac{dx}{dt}, \frac{dy}{dt} \right\rangle = \langle 4t, 9t^2 \rangle$$

**Magnitude of Velocity (Speed) $|\vec{v}(t)|$:**
$$|\vec{v}(t)| = \sqrt{(4t)^2 + (9t^2)^2} = \sqrt{16t^2 + 81t^4} = t\sqrt{16 + 81t^2}$$

### Acceleration $\vec{a}(t)$
$$\vec{a}(t) = \frac{d\vec{v}}{dt} = \langle 4, 18t \rangle$$

**Magnitude of Acceleration $|\vec{a}(t)|$:**
$$|\vec{a}(t)| = \sqrt{4^2 + (18t)^2} = \sqrt{16 + 324t^2} = 2\sqrt{4 + 81t^2}$$

---

## 5. Interpretation of Acceleration
**Is the acceleration constant?**
No. 

While the $x$-component of acceleration ($a_x = 4$) is constant, the $y$-component ($a_y = 18t$) depends linearly on time. Therefore, the total acceleration vector $\vec{a}(t)$ changes in both magnitude and direction as $t$ progresses.

---

## Summary Table
| Parameter | Expression |
| :--- | :--- |
| **Path Equation** | $y = \frac{3}{2\sqrt{2}}x^{3/2}$ |
| **Velocity Vector** | $\vec{v}(t) = 4t\hat{i} + 9t^2\hat{j}$ |
| **Acceleration Vector** | $\vec{a}(t) = 4\hat{i} + 18t\hat{j}$ |
| **Constant Acceleration?** | **No** |