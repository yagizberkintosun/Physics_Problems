## 8. Waves

#### **1. The Traveling Wave Condition**
For a function to describe a traveling wave, it must be a valid solution to the linear wave equation:
$$\frac{\partial^2 y}{\partial x^2} = \frac{1}{v^2} \frac{\partial^2 y}{\partial t^2}$$

A shortcut in physics is to check if the function can be written entirely in the form of $f(x \pm vt)$. Let's prove this by testing the partial derivatives of each option as the hint suggests.

#### **2. Test Option A: $y(x,t) = A \cos(kx^2 - \omega t)$**
Let's take the second partial derivative with respect to position ($x$):
$$\frac{\partial y}{\partial x} = -A \sin(kx^2 - \omega t) \cdot (2kx)$$
$$\frac{\partial^2 y}{\partial x^2} = -2Ak \sin(kx^2 - \omega t) - 4Ak^2x^2 \cos(kx^2 - \omega t)$$

Now, the second partial derivative with respect to time ($t$):
$$\frac{\partial y}{\partial t} = -A \sin(kx^2 - \omega t) \cdot (-\omega) = A\omega \sin(kx^2 - \omega t)$$
$$\frac{\partial^2 y}{\partial t^2} = -A\omega^2 \cos(kx^2 - \omega t)$$

**Conclusion for A:** Because the spatial derivative ($\frac{\partial^2 y}{\partial x^2}$) has an extra sine term and an $x^2$ coefficient, it does not equal $\frac{1}{v^2}\frac{\partial^2 y}{\partial t^2}$. 
**Function A is NOT a traveling wave.**

#### **3. Test Option B: $y(x,t) = A(x - vt)^2$**
Let's find the spatial derivatives:
$$\frac{\partial y}{\partial x} = 2A(x - vt)$$
$$\frac{\partial^2 y}{\partial x^2} = 2A$$

Now the time derivatives:
$$\frac{\partial y}{\partial t} = 2A(x - vt) \cdot (-v) = -2Av(x - vt)$$
$$\frac{\partial^2 y}{\partial t^2} = -2Av \cdot (-v) = 2Av^2$$

Plug these into the wave equation:
$$2A = \frac{1}{v^2} (2Av^2)$$
$$2A = 2A$$

**Conclusion for B:** The two sides are perfectly equal. 
**Function B satisfies the wave equation.**

#### **4. Test Option C: $y(x,t) = A \log(x + vt)$**
Let's find the spatial derivatives:
$$\frac{\partial y}{\partial x} = \frac{A}{x + vt}$$
$$\frac{\partial^2 y}{\partial x^2} = -\frac{A}{(x + vt)^2}$$

Now the time derivatives:
$$\frac{\partial y}{\partial t} = \frac{A}{x + vt} \cdot (v) = \frac{Av}{x + vt}$$
$$\frac{\partial^2 y}{\partial t^2} = -\frac{Av}{(x + vt)^2} \cdot (v) = -\frac{Av^2}{(x + vt)^2}$$

Plug these into the wave equation:
$$-\frac{A}{(x + vt)^2} = \frac{1}{v^2} \left( -\frac{Av^2}{(x + vt)^2} \right)$$
$$-\frac{A}{(x + vt)^2} = -\frac{A}{(x + vt)^2}$$

**Conclusion for C:** The two sides are perfectly equal.
**Function C satisfies the wave equation.**

#### **Final Answer**
**Options b) and c)** both satisfy the mathematical wave equation because their arguments are in the form of $(x \pm vt)$. *(Note: While they are mathematically valid solutions to the differential equation, physical traveling waves are usually bounded functions like sine or cosine, whereas polynomials and logs grow to infinity).*