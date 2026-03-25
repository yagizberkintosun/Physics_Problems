# Path Intersection and Collision Analysis


This document outlines the analytical approach to determine if two moving objects, Alice and Bob, will collide, if their paths intersect at different times, or the minimum distance between them if they never meet.

---

## 1. Defining the Paths


Let the positions of Alice and Bob at time $t$ be represented by the following vector-valued functions:


* **Alice:** $\mathbf{r}_A(t) = \langle x_A(t), y_A(t), z_A(t) \rangle$
* **Bob:** $\mathbf{r}_B(t) = \langle x_B(t), y_B(t), z_B(t) \rangle$


---

## 2. Determining Collision


A **collision** occurs if Alice and Bob are at the exact same coordinates at the exact same time $t$. To find this, we set the components equal to each other:


1.  $x_A(t) = x_B(t)$
2.  $y_A(t) = y_B(t)$
3.  $z_A(t) = z_B(t)$

If there is a value of $t \ge 0$ that satisfies all three equations simultaneously, then:
* **Time of collision:** $t$
* **Location of collision:** $\mathbf{r}_A(t)$

---

## 3. Determining Path Intersection


An **intersection** occurs if their paths cross, even if they aren't there at the same time. We check this by using two different time variables, $t_1$ and $t_2$:

$$\mathbf{r}_A(t_1) = \mathbf{r}_B(t_2)$$

If a solution exists for $t_1$ and $t_2$, the paths intersect at the point $\mathbf{r}_A(t_1)$, but the objects do not necessarily collide.

---

## 4. Minimum Distance (Closest Approach)


If no collision occurs, we find the minimum distance between them by defining a distance function $d(t)$:

$$d(t) = |\mathbf{r}_A(t) - \mathbf{r}_B(t)|$$
$$d(t) = \sqrt{(x_A-x_B)^2 + (y_A-y_B)^2 + (z_A-z_B)^2}$$

### Optimization Steps:

1.  Define $f(t) = [d(t)]^2$ to avoid dealing with the square root.
2.  Find the derivative $f'(t)$.
3.  Set $f'(t) = 0$ and solve for $t$.
4.  Plug this $t$ back into $d(t)$ to find the **minimum distance**.

---

## 5. Summary of Results


| Condition | Mathematical Requirement | Result |
| :--- | :--- | :--- |
| **Collision** | $\mathbf{r}_A(t) = \mathbf{r}_B(t)$ | [Input Result] |
| **Intersection** | $\mathbf{r}_A(t_1) = \mathbf{r}_B(t_2)$ | [Input Result] |
| **Min Distance** | $\frac{d}{dt} |\mathbf{r}_A(t) - \mathbf{r}_B(t)| = 0$ | [Input Result] |