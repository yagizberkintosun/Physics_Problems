## 8. Definite Integrals: Area Under the Curve

**Problem Statement:**
Calculate the area under the curve of the function $f(x) = \sin(x)$ from $x=0$ to $x=\pi$.



---

### Step 1: Set up the Definite Integral
The area $A$ under a curve $f(x)$ from $a$ to $b$ is given by the integral:
$$A = \int_{a}^{b} f(x) \, dx$$

For this problem:
$$A = \int_{0}^{\pi} \sin(x) \, dx$$

### Step 2: Find the Antiderivative
The antiderivative of $\sin(x)$ is $-\cos(x)$. We apply the Fundamental Theorem of Calculus:
$$A = \left[ -\cos(x) \right]_{0}^{\pi}$$

### Step 3: Evaluate at the Boundaries
Substitute the upper limit ($\pi$) and subtract the lower limit ($0$):
$$A = (-\cos(\pi)) - (-\cos(0))$$

Recall the trigonometric values:
* $\cos(\pi) = -1$
* $\cos(0) = 1$

$$A = (-(-1)) - (-1)$$
$$A = 1 + 1$$
$$\mathbf{A = 2}$$

---

### Conclusion
The total area under one hump of the sine curve from $0$ to $\pi$ is exactly **2 square units**.