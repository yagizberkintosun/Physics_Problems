# Section 0 — Mathematical Foundations  
## 1. Vector Algebra
# Section 0: Mathematical Foundations - Solutions

## 1. Vector Algebra

Given the vectors:
* $\vec{a} = [2, 1, -3]$
* $\vec{b} = [4, -2, 1]$

---

### a) Magnitude of each vector
The magnitude is calculated using the formula $|\vec{v}| = \sqrt{x^2 + y^2 + z^2}$.

**Magnitude of $\vec{a}$:**
$$|\vec{a}| = \sqrt{2^2 + 1^2 + (-3)^2} = \sqrt{4 + 1 + 9} = \sqrt{14} \approx 3.742$$

**Magnitude of $\vec{b}$:**
$$|\vec{b}| = \sqrt{4^2 + (-2)^2 + 1^2} = \sqrt{16 + 4 + 1} = \sqrt{21} \approx 4.583$$

---

### b) Dot Product ($\vec{a} \cdot \vec{b}$)
The dot product is the sum of the products of the components:
$$\vec{a} \cdot \vec{b} = (a_x \cdot b_x) + (a_y \cdot b_y) + (a_z \cdot b_z)$$
$$\vec{a} \cdot \vec{b} = (2 \times 4) + (1 \times -2) + (-3 \times 1)$$
$$\vec{a} \cdot \vec{b} = 8 - 2 - 3 = \mathbf{3}$$

---

### c) Cross Product ($\vec{a} \times \vec{b}$)
The cross product is found using the determinant of the unit vector matrix:



$$\vec{a} \times \vec{b} = \begin{vmatrix} \mathbf{i} & \mathbf{j} & \mathbf{k} \\ 2 & 1 & -3 \\ 4 & -2 & 1 \end{vmatrix}$$

* **i-component:** $(1 \times 1) - (-3 \times -2) = 1 - 6 = -5$
* **j-component:** $-( (2 \times 1) - (-3 \times 4) ) = -(2 + 12) = -14$
* **k-component:** $(2 \times -2) - (1 \times 4) = -4 - 4 = -8$

**Result:** $\vec{a} \times \vec{b} = [-5, -14, -8]$

---

### d) Angle between vectors
Using the relationship $\vec{a} \cdot \vec{b} = |\vec{a}| |\vec{b}| \cos(\theta)$:

$$\cos(\theta) = \frac{\vec{a} \cdot \vec{b}}{|\vec{a}| |\vec{b}|}$$
$$\cos(\theta) = \frac{3}{\sqrt{14} \cdot \sqrt{21}} = \frac{3}{\sqrt{294}} \approx 0.175$$

**Angle $\theta$:**
* $\theta \approx 1.395 \text{ radians}$
* $\theta \approx 79.92^\circ$