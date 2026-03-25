# Path Intersection and Collision Analysis

This document evaluates the trajectories of Alice and Bob to determine if a collision occurs or to find the minimum distance between them.

---

## 1. Trajectory Equations
The positions of Alice ($\mathbf{A}$) and Bob ($\mathbf{B}$) at time $t$ are:
* $\mathbf{A}(t) = (2 + t, 8 - 3t)$
* $\mathbf{B}(t) = (2t - 1, 2t + 2)$

---

## 2. Collision Check
A collision occurs only if Alice and Bob occupy the same coordinates at the **same time** $t$.

**Equating $x$-components:**
$$2 + t = 2t - 1 \implies t = 3$$

**Equating $y$-components:**
$$8 - 3t = 2t + 2 \implies 6 = 5t \implies t = 1.2$$

Since the times required for the components to match are different ($3 \neq 1.2$), **Alice and Bob do not collide.**

---

## 3. Path Intersection Check
The paths themselves intersect if there exist times $t_1$ and $t_2$ such that $\mathbf{A}(t_1) = \mathbf{B}(t_2)$.

1.  $2 + t_1 = 2t_2 - 1 \implies t_1 = 2t_2 - 3$
2.  $8 - 3t_1 = 2t_2 + 2$

Substituting (1) into (2):
$$8 - 3(2t_2 - 3) = 2t_2 + 2$$
$$17 - 6t_2 = 2t_2 + 2 \implies 8t_2 = 15 \implies t_2 = 1.875$$
$$t_1 = 2(1.875) - 3 = 0.75$$

**Intersection Point:**
Plugging $t_1 = 0.75$ into $\mathbf{A}(t)$:
$$x = 2 + 0.75 = 2.75, \quad y = 8 - 3(0.75) = 5.75$$
The paths intersect at **$(2.75, 5.75)$**, but since $t_1 \neq t_2$, no collision occurs.

---

## 4. Minimum Distance Calculation
Since they do not collide, we find the minimum distance $D(t)$ by optimizing the distance squared function $f(t)$:

$$f(t) = [x_A(t) - x_B(t)]^2 + [y_A(t) - y_B(t)]^2$$
$$f(t) = [(2 + t) - (2t - 1)]^2 + [(8 - 3t) - (2t + 2)]^2$$
$$f(t) = (3 - t)^2 + (6 - 5t)^2$$
$$f(t) = 26t^2 - 66t + 45$$

**Finding the Minimum:**
Set the first derivative $f'(t)$ to zero:
$$f'(t) = 52t - 66 = 0 \implies t = \frac{33}{26} \approx 1.269 \text{ s}$$

**Minimum Distance Value:**
$$D_{min} = \sqrt{f(1.269)} = \sqrt{\frac{81}{26}} \approx 1.765 \text{ units}$$

---

## Summary of Results
| Condition | Result |
| :--- | :--- |
| **Collision?** | No |
| **Path Intersection?** | Yes, at $(2.75, 5.75)$ |
| **Minimum Distance** | $\approx 1.765$ units |
| **Time of Min Distance** | $\approx 1.269$ seconds |