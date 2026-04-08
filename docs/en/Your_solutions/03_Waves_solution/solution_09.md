## 9. Damped Oscillator

#### **1. General Solution & 2. Classification of Cases**
The differential equation for a damped harmonic oscillator is:
$$m \frac{d^2x}{dt^2} + b \frac{dx}{dt} + kx = 0$$

To find the general solution, we assume a solution of the form $x(t) = e^{rt}$, which gives us the characteristic equation:
$$mr^2 + br + k = 0$$

Using the quadratic formula, the roots are:
$$r = \frac{-b \pm \sqrt{b^2 - 4mk}}{2m}$$

The physical behavior of the system depends entirely on the term under the square root ($b^2 - 4mk$):

* **Underdamped ($b^2 < 4mk$):** The roots are complex. The system oscillates back and forth, but the amplitude slowly decays over time due to friction/damping.
  $$x(t) = A e^{-\frac{b}{2m} t} \cos(\omega_d t + \phi)$$
  
* **Critically Damped ($b^2 = 4mk$):** The roots are real and equal. The system returns to its resting point as quickly as mathematically possible without ever crossing zero (no oscillation).
  $$x(t) = (A + Bt) e^{-\frac{b}{2m} t}$$
  
* **Overdamped ($b^2 > 4mk$):** The roots are real and distinct. The damping is so strong that the system behaves like it's moving through thick honey, returning to zero very slowly without oscillating.
  $$x(t) = A e^{r_1 t} + B e^{r_2 t}$$

#### **3. Numerical Solution (RK4 Setup)**
To solve this differential equation numerically in code (like using the 4th-Order Runge-Kutta method), we must reduce the 2nd-order equation into a system of two 1st-order equations. 

We define velocity as $v = \frac{dx}{dt}$. Substituting this into our original equation gives us our system:
1. $\frac{dx}{dt} = v$
2. $\frac{dv}{dt} = -\frac{b}{m}v - \frac{k}{m}x$

*(Note: The actual implementation of the RK4 algorithm, the parameter investigation, the $x(t)$ graph, and the phase portrait are deployed in the interactive simulation).*