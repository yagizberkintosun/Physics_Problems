## 12. Work and Energy with a Constant Force

#### **1. Determine Acceleration ($\vec{a}(t)$)**
Using Newton's Second Law ($\vec{F} = m\vec{a}$):
$$\vec{a}(t) = \frac{\vec{F}}{m} = \frac{[6, 2]}{2}$$
**$$\vec{a}(t) = [3, 1]\text{ m/s}^2$$**

#### **2. Determine Velocity ($\vec{v}(t)$)**
Velocity is the integral of acceleration:
$$\vec{v}(t) = \int \vec{a}(t) \, dt = \left[ \int 3 \, dt, \int 1 \, dt \right]$$
$$\vec{v}(t) = [3t + C_x, t + C_y]$$
Applying the initial condition $\vec{v}(0) = [1, -1]$:
**$$\vec{v}(t) = [3t + 1, t - 1]\text{ m/s}$$**

#### **3. Determine Position ($\vec{r}(t)$)**
Position is the integral of velocity:
$$\vec{r}(t) = \int \vec{v}(t) \, dt = \left[ \int (3t + 1) \, dt, \int (t - 1) \, dt \right]$$
$$\vec{r}(t) = \left[ 1.5t^2 + t + C_x, 0.5t^2 - t + C_y \right]$$
Applying the initial condition $\vec{r}(0) = [0, 0]$:
**$$\vec{r}(t) = [1.5t^2 + t, 0.5t^2 - t]\text{ m}$$**

#### **4. Trajectory of the Motion**
The trajectory is a parabola derived by plotting the $y(t)$ position against the $x(t)$ position. 
*(You can generate this plot using the Python snippet at the bottom of this file).*

#### **5. Calculate Work Done at $t = 3$ s**
Work is the dot product of Force and Displacement ($W = \vec{F} \cdot \Delta\vec{r}$).
First, find the displacement at $t = 3$:
$$\vec{r}(3) = [1.5(3)^2 + 3, 0.5(3)^2 - 3]$$
$$\vec{r}(3) = [1.5(9) + 3, 0.5(9) - 3] = [13.5 + 3, 4.5 - 3]$$
$$\vec{r}(3) = [16.5, 1.5]\text{ m}$$

Since the starting position is the origin, $\Delta\vec{r} = [16.5, 1.5]$.
$$W = [6, 2] \cdot [16.5, 1.5]$$
$$W = (6 \cdot 16.5) + (2 \cdot 1.5) = 99 + 3$$
**$$W = 102\text{ J}$$**

#### **6. Work-Energy Theorem Consistency Check**
The work-energy theorem states $W = \Delta K = K_f - K_i$.
First, calculate the initial kinetic energy ($K_i$) at $t = 0$:
$$\vec{v}(0) = [1, -1]$$
$$|\vec{v}(0)|^2 = (1)^2 + (-1)^2 = 2$$
$$K_i = \frac{1}{2}mv_i^2 = \frac{1}{2}(2)(2) = 2\text{ J}$$

Next, calculate the final kinetic energy ($K_f$) at $t = 3$:
$$\vec{v}(3) = [3(3) + 1, 3 - 1] = [10, 2]$$
$$|\vec{v}(3)|^2 = (10)^2 + (2)^2 = 100 + 4 = 104$$
$$K_f = \frac{1}{2}mv_f^2 = \frac{1}{2}(2)(104) = 104\text{ J}$$

Finally, verify the change in kinetic energy:
$$\Delta K = K_f - K_i = 104 - 2 = 102\text{ J}$$

**Conclusion:** The work calculated via the dot product (102 J) perfectly matches the change in kinetic energy (102 J), verifying the work-energy theorem.

---

### **Trajectory Plotting Code (Python)**
```python
import numpy as np
import matplotlib.pyplot as plt

# Time vector from 0 to 3 seconds
t = np.linspace(0, 3, 100)

# Parametric equations for x and y
x = 1.5 * t**2 + t
y = 0.5 * t**2 - t

# Plotting the trajectory
plt.figure(figsize=(8, 5))
plt.plot(x, y, label='Trajectory', color='purple', linewidth=2)
plt.scatter([0], [0], color='black', zorder=5, label='Start (t=0)')
plt.scatter([16.5], [1.5], color='red', zorder=5, label='End (t=3)')

plt.title('Particle Trajectory from t=0 to t=3')
plt.xlabel('Position x (m)')
plt.ylabel('Position y (m)')
plt.axhline(0, color='gray', linestyle='--')
plt.axvline(0, color='gray', linestyle='--')
plt.grid(True)
plt.legend()
plt.show()