## 2. Electric Potential: System of Point Charges

#### **1. Identify the Physical System**
* **Charges:** $q_1 = +1\text{ C}, q_2 = -2\text{ C}, q_3 = +3\text{ C}, q_4 = -4\text{ C}$.
* **Geometry:** Corners of a square with side length $s = 1.0\text{ m}$.
* **Target:** Electric Potential ($V$) at the center of the square.

#### **2. Geometric Analysis**
The electric potential $V$ at a point depends on the distance ($r$) from the source charge. For a square, the distance from any corner to the center is half the diagonal:
1. Diagonal ($d$): $s\sqrt{2} = 1.0 \cdot \sqrt{2}\text{ m}$
2. Distance ($r$): $\frac{d}{2} = \frac{\sqrt{2}}{2} \approx 0.707\text{ m}$

#### **3. The Scalar Nature of Potential**
Unlike Electric Force (which is a **vector**), Electric Potential is a **scalar** quantity. This means direction does not matter. We do not need to worry about $x$ and $y$ components or angles. We simply calculate the potential from each charge and sum them algebraically:
$$V_{total} = V_1 + V_2 + V_3 + V_4$$

#### **4. Mathematical Solution**
The formula for potential from a point charge is $V = \frac{kq}{r}$. Since $k$ and $r$ are the same for all four charges, we can factor them out to simplify the calculation:
$$V_{total} = \frac{k}{r} (q_1 + q_2 + q_3 + q_4)$$

1. Sum of charges: $1\text{ C} - 2\text{ C} + 3\text{ C} - 4\text{ C} = -2\text{ C}$
2. Substitute values:
$$V_{total} = \frac{8.99 \times 10^9}{-2 / (\sqrt{2}/2)}$$
$$V_{total} = (8.99 \times 10^9) \cdot \frac{-2}{0.7071}$$

**Final Result:**
**$V_{total} \approx -2.54 \times 10^{10}\text{ V}$**