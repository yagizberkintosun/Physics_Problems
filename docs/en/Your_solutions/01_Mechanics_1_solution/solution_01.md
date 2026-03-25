# Projectile Motion Analysis

This document provides the derivation of the fundamental equations for a projectile fired from the ground with an initial velocity $v_0$ at an angle $\theta$ above the horizontal. Assume no air resistance.

---

## 1. Differential Equations of Motion

We assume the only force acting on the projectile is gravity acting in the negative $y$ direction.



### Initial Conditions
* **Initial Position:** $(x_0, y_0) = (0, 0)$
* **Initial Velocity Components:**
    * $v_{x0} = v_0 \cos \theta$
    * $v_{y0} = v_0 \sin \theta$


### Accelerations
The acceleration components are:
$$\frac{d^2x}{dt^2} = 0$$
$$\frac{d^2y}{dt^2} = -g$$


### Velocities
Integrating the acceleration with respect to time $t$:
* $v_x(t) = v_0 \cos \theta$
* $v_y(t) = v_0 \sin \theta - gt$


### Positions
Integrating the velocity with respect to time $t$:
* $x(t) = (v_0 \cos \theta)t$
* $y(t) = (v_0 \sin \theta)t - \frac{1}{2}gt^2$


---

## 2. Time of Flight ($T$)

The time of flight is the total time the projectile remains in the air. This occurs when the vertical displacement returns to zero ($y = 0$).

$$0 = (v_0 \sin \theta)T - \frac{1}{2}gT^2$$

Factoring out $T$:
$$T \left( v_0 \sin \theta - \frac{1}{2}gT \right) = 0$$

Since $T > 0$ at the end of the flight:
$$T = \frac{2 v_0 \sin \theta}{g}$$

---

## 3. Maximum Height ($H$)

The maximum height is reached when the vertical velocity component becomes zero ($v_y = 0$).

$$v_y = v_0 \sin \theta - gt_{peak} = 0$$
$$t_{peak} = \frac{v_0 \sin \theta}{g}$$

Substituting $t_{peak}$ into the equation for $y(t)$:
$$H = (v_0 \sin \theta) \left( \frac{v_0 \sin \theta}{g} \right) - \frac{1}{2}g \left( \frac{v_0 \sin \theta}{g} \right)^2$$
$$H = \frac{v_0^2 \sin^2 \theta}{2g}$$

---

## 4. Range ($R$)

The range is the total horizontal distance traveled during the time of flight $T$.

$$R = x(T) = (v_0 \cos \theta)T$$

Substituting the expression for $T$:
$$R = (v_0 \cos \theta) \left( \frac{2 v_0 \sin \theta}{g} \right)$$
$$R = \frac{v_0^2 (2 \sin \theta \cos \theta)}{g}$$

Using the trigonometric identity $2 \sin \theta \cos \theta = \sin(2\theta)$:
$$R = \frac{v_0^2 \sin(2\theta)}{g}$$
