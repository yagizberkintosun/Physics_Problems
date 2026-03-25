# Range Optimization Analysis


This document provides the analytical derivation to determine the launch angle $\theta$ that yields the maximum horizontal range $R$ for a projectile with a given initial velocity $v_0$.

---

## 1. The Range Equation


From the basic equations of projectile motion (assuming no air resistance and a level landing surface), the horizontal range $R$ is given by:


$$R = \frac{v_0^2 \sin(2\theta)}{g}$$

Where:
* $v_0$ is the initial velocity.
* $\theta$ is the launch angle.
* $g$ is the acceleration due to gravity.

---

## 2. Analytical Optimization


To find the angle $\theta$ that maximizes $R$, we take the first derivative of $R$ with respect to $\theta$ and set it to zero.


### Step 1: Differentiate $R(\theta)$


Using the chain rule:
$$\frac{dR}{d\theta} = \frac{d}{d\theta} \left( \frac{v_0^2 \sin(2\theta)}{g} \right)$$
$$\frac{dR}{d\theta} = \frac{v_0^2}{g} \cdot \cos(2\theta) \cdot 2$$
$$\frac{dR}{d\theta} = \frac{2v_0^2 \cos(2\theta)}{g}$$


### Step 2: Set the derivative to zero

To find the critical points, we set $\frac{dR}{d\theta} = 0$:
$$0 = \frac{2v_0^2 \cos(2\theta)}{g}$$

Since $v_0$ and $g$ are non-zero constants:
$$\cos(2\theta) = 0$$

### Step 3: Solve for $\theta$


The cosine function is zero when its argument is $90^\circ$ (or $\frac{\pi}{2}$ radians):
$$2\theta = 90^\circ$$
$$\theta = 45^\circ$$

---

## 3. Conclusion

By setting the derivative of the range equation to zero, we find that the maximum range is achieved when:
$$\theta = 45^\circ$$

At this angle, $\sin(2\theta) = \sin(90^\circ) = 1$, which is the maximum possible value for the sine function, resulting in the maximum range:
$$R_{max} = \frac{v_0^2}{g}$$