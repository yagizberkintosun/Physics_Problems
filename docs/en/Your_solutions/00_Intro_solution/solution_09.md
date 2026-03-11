## 9. Optimization Problem: Maximum Area Rectangle

**Problem Statement:**
A rectangle is placed in the first quadrant with one vertex at the origin $(0,0)$, one on the x-axis, one on the y-axis, and the opposite vertex on the curve $y = 3 - x^2$. Find the dimensions $(x, y)$ that maximize the area.



---

### Step 1: Define the Area Function
The area $A$ of a rectangle with width $x$ and height $y$ is:
$$A = x \cdot y$$

Since the point $(x, y)$ lies on the curve $y = 3 - x^2$, we substitute $y$:
$$A(x) = x(3 - x^2)$$
$$A(x) = 3x - x^3$$

### Step 2: Find the Critical Points
To find the maximum area, take the derivative of $A(x)$ with respect to $x$ and set it to zero:
$$A'(x) = \frac{d}{dx}(3x - x^3)$$
$$A'(x) = 3 - 3x^2$$

Set $A'(x) = 0$:
$$3 - 3x^2 = 0$$
$$3x^2 = 3$$
$$x^2 = 1$$
$$\mathbf{x = 1} \text{ (since we are in the first quadrant, } x > 0\text{)}$$

### Step 3: Verify it is a Maximum
Using the second derivative test:
$$A''(x) = -6x$$
At $x = 1$, $A''(1) = -6$. Since the second derivative is negative, the area is at a **local maximum**.

### Step 4: Calculate the Dimensions
* **Width:** $x = 1$
* **Height:** Substitute $x = 1$ into the curve equation:
  $$y = 3 - (1)^2 = \mathbf{2}$$

---

### Conclusion
The dimensions of the rectangle with the maximum area are:
* **Width:** $1$
* **Height:** $2$

The maximum area is **2 square units**.