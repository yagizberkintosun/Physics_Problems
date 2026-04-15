# Problem 6: Electric Field Analysis of a Two-Charge System

### 1. System Configuration
We have two point charges located on the x-axis:
* $q_1 = +q$ at position $\vec{r}_1 = (-a, 0)$
* $q_2 = +2q$ at position $\vec{r}_2 = (a, 0)$

The electric field at any point $P(x, y)$ is the vector sum of the fields from both charges:
$$\vec{E}_{total} = \vec{E}_1 + \vec{E}_2 = k \frac{q_1}{r_1^3}\vec{r}_{P/1} + k \frac{q_2}{r_2^3}\vec{r}_{P/2}$$

---

### 2. General Field Vector $\vec{E}(x, y)$
Let the point of interest be $(x, y)$.
* Displacement from $q_1$: $\vec{r}_{P/1} = (x - (-a))\hat{i} + (y - 0)\hat{j} = (x + a)\hat{i} + y\hat{j}$
* Magnitude: $r_1 = \sqrt{(x + a)^2 + y^2}$
* Displacement from $q_2$: $\vec{r}_{P/2} = (x - a)\hat{i} + (y - 0)\hat{j} = (x - a)\hat{i} + y\hat{j}$
* Magnitude: $r_2 = \sqrt{(x - a)^2 + y^2}$

The general expression is:
$$\vec{E}(x, y) = kq \left[ \frac{(x + a)\hat{i} + y\hat{j}}{((x + a)^2 + y^2)^{3/2}} + \frac{2((x - a)\hat{i} + y\hat{j})}{((x - a)^2 + y^2)^{3/2}} \right]$$

#### Specific Field $\vec{E}(0, y)$:
At $x = 0$, both distances are equal: $r_1 = r_2 = \sqrt{a^2 + y^2}$.
$$\vec{E}(0, y) = \frac{kq}{(a^2 + y^2)^{3/2}} \left[ (a\hat{i} + y\hat{j}) + 2(-a\hat{i} + y\hat{j}) \right]$$
$$\vec{E}(0, y) = \frac{kq}{(a^2 + y^2)^{3/2}} (-a\hat{i} + 3y\hat{j})$$

#### Specific Field $\vec{E}(x, 0)$:
At $y = 0$, the $\hat{j}$ components vanish:
$$\vec{E}(x, 0) = kq \left[ \frac{x+a}{|x+a|^3} + \frac{2(x-a)}{|x-a|^3} \right] \hat{i}$$

---

### 3. Conditions for Zero Field ($\vec{E} = 0$)
For the total field to be zero, both $E_x$ and $E_y$ must be zero.
* From our $\vec{E}(0, y)$ derivation, $E_y$ is only zero if $y=0$ (on the x-axis).
* On the x-axis, between the charges (where $-a < x < a$):
$$\frac{1}{(x+a)^2} = \frac{2}{(a-x)^2}$$
Taking the square root: $\frac{1}{x+a} = \frac{\sqrt{2}}{a-x}$
$$a - x = \sqrt{2}x + \sqrt{2}a \implies x = a \frac{1-\sqrt{2}}{1+\sqrt{2}} \approx -0.171a$$

---

### 4. Numerical Calculation
**Given:** $a = 0.2\text{m}$, $y = 0.3\text{m}$, $q = 2\mu\text{C}$ (Assuming point $(0, y)$).
* $r = \sqrt{0.2^2 + 0.3^2} = \sqrt{0.13} \approx 0.3606\text{m}$
* $k = 8.99 \times 10^9$
* Using $\vec{E}(0, y) = \frac{kq}{r^3}(-a\hat{i} + 3y\hat{j})$:
  * $E_x = \frac{(8.99 \times 10^9)(2 \times 10^{-6})}{(0.13)^{3.5}} \times (-0.2) \approx -7.67 \times 10^4 \text{ N/C}$
  * $E_y = \frac{(8.99 \times 10^9)(2 \times 10^{-6})}{(0.13)^{1.5}} \times (0.9) \approx 3.45 \times 10^5 \text{ N/C}$

---

### 5. Limit Analysis ($y \gg a$)
As $y$ becomes very large compared to $a$, the terms $(a^2 + y^2)$ simply become $y^2$.
$$\vec{E}(0, y) \approx \frac{kq}{(y^2)^{3/2}} (-a\hat{i} + 3y\hat{j}) \approx \frac{3kqy}{y^3}\hat{j} = \frac{k(3q)}{y^2}\hat{j}$$
This shows the system behaves like a single point charge of magnitude $3q$ at the origin.