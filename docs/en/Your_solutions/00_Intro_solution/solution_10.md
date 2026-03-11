## 10. Infinite Series: The Ant's Path

**Problem Statement:**
An ant moves in a repeating pattern of East, North, West, South, with decreasing step sizes ($1, 1/2, 1/3, 1/4, \dots$). Find the final $(x, y)$ coordinates.

[Image of a spiral path on a coordinate plane representing an infinite series of movements]

---

### Step 1: Analyze the Horizontal Movement ($x$)
The ant moves East ($+$) and West ($-$) on every odd-numbered step:
* Step 1: $+1$
* Step 3: $-1/3$
* Step 5: $+1/5$
* ...and so on.

The x-coordinate is the sum of the series:
$$x = 1 - \frac{1}{3} + \frac{1}{5} - \frac{1}{7} + \dots$$

This is a famous series related to the Taylor expansion of $\arctan(x)$. Specifically, $\arctan(1) = 1 - \frac{1}{3} + \frac{1}{5} - \dots$.
Since $\arctan(1) = \frac{\pi}{4}$:
$$\mathbf{x = \frac{\pi}{4} \approx 0.785}$$

---

### Step 2: Analyze the Vertical Movement ($y$)
The ant moves North ($+$) and South ($-$) on every even-numbered step:
* Step 2: $+1/2$
* Step 4: $-1/4$
* Step 6: $+1/6$
* ...and so on.

The y-coordinate is the sum of the series:
$$y = \frac{1}{2} - \frac{1}{4} + \frac{1}{6} - \frac{1