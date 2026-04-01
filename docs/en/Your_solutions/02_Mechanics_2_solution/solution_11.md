## 11. Dynamics with a time-dependent force


#### **1. Find the Acceleration ($\mathbf{a}(t)$)**
Using Newton's Second Law ($\mathbf{F} = m\mathbf{a}$), we divide the force vector by the mass ($m = 3\text{ kg}$):
$$\mathbf{a}(t) = \frac{\mathbf{F}(t)}{m} = \frac{(15t, 3t - 12, -6t^2)}{3}$$
$$\mathbf{a}(t) = (5t, t - 4, -2t^2)\text{ m/s}^2$$

#### **2. Find the Velocity ($\mathbf{v}(t)$)**
Velocity is the integral of acceleration with respect to time ($\mathbf{v} = \int \mathbf{a} \, dt$):
* $v_x(t) = \int 5t \, dt = \frac{5}{2}t^2 + C_{1x}$
* $v_y(t) = \int (t - 4) \, dt = \frac{1}{2}t^2 - 4t + C_{1y}$
* $v_z(t) = \int -2t^2 \, dt = -\frac{2}{3}t^3 + C_{1z}$

We apply the initial condition $\mathbf{v}(0) = (2, 0, 1)$ to find the constants:
* $v_x(0) = C_{1x} = 2$
* $v_y(0) = C_{1y} = 0$
* $v_z(0) = C_{1z} = 1$

**The velocity vector is:**
$$\mathbf{v}(t) = \left( \frac{5}{2}t^2 + 2, \, \frac{1}{2}t^2 - 4t, \, -\frac{2}{3}t^3 + 1 \right)\text{ m/s}$$

