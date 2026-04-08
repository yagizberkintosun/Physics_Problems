## 3. Superposition Principle

#### **1. Set up the Superposition Equation**
The principle of superposition states that the resulting wave is simply the sum of the individual waves:
$$y(x,t) = y_1(x,t) + y_2(x,t)$$
$$y(x,t) = A \sin(kx - \omega t) + A \sin(kx + \omega t)$$

#### **2. Apply Trigonometric Identities**
To simplify this into a single readable equation, we use the sum-to-product trigonometric identity:
$$\sin(\alpha - \beta) + \sin(\alpha + \beta) = 2 \sin(\alpha) \cos(\beta)$$

By substituting $\alpha = kx$ and $\beta = \omega t$, we get the final equation for the standing wave:
**$$y(x,t) = 2A \sin(kx) \cos(\omega t)$$**

#### **3. Identify the Positions of the Nodes**
Nodes are the specific points on a standing wave that never move (amplitude is always zero). This happens when the spatial part of our new equation is equal to zero:
$$2A \sin(kx) = 0 \implies \sin(kx) = 0$$

For sine to equal zero, the inside ($kx$) must be an integer multiple of $\pi$:
$$kx = n\pi \quad (\text{where } n = 0, 1, 2, 3, \dots)$$

Since we know the wave number $k$ is equal to $\frac{2\pi}{\lambda}$, we can substitute that in to find the physical positions ($x$):
$$\left(\frac{2\pi}{\lambda}\right) x = n\pi$$

Solving for $x$, the $\pi$ on both sides cancels out, leaving us with:
**$$x = \frac{n\lambda}{2}$$**

*(Conclusion: The nodes are located at every half-wavelength: $0, \frac{\lambda}{2}, \lambda, \frac{3\lambda}{2}, \dots$)*