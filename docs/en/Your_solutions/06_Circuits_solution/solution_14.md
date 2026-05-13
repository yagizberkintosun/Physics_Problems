# Physics Problem: RLC Circuit Differential Equation and Mechanical Analogies

## 1. Problem Statement
We are required to:
1.  Derive the differential equation for a series RLC circuit containing a voltage source ($V$), a resistor ($R$), an inductor ($L$), and a capacitor ($C$).
2.  Express the equation in terms of the voltage across the capacitor ($V_C(t)$).
3.  Compare the result to the equation of a damped harmonic oscillator.
4.  Identify the physical analogies between the two systems.

---

## 2. Deriving the RLC Differential Equation

### Step A: Kirchhoff’s Voltage Law (KVL)
For a series loop, the sum of the potential differences across each component must equal the source voltage:
$$V(t) = V_L(t) + V_R(t) + V_C(t)$$

Substituting the defining equations for each component:
*   Voltage across inductor: $V_L = L \frac{dI}{dt}$
*   Voltage across resistor: $V_R = R I$
*   Voltage across capacitor: $V_C$

We get:
$$L \frac{dI(t)}{dt} + R I(t) + V_C(t) = V(t) \quad \text{--- (Eq. 1)}$$

### Step B: Relating Current to Capacitor Voltage
The current ($I$) in the circuit is the rate of change of charge on the capacitor ($I = \frac{dq}{dt}$). Since $q = C V_C$, we can relate current directly to $V_C$:
$$I(t) = C \frac{dV_C(t)}{dt}$$

Taking the derivative of the current to find $\frac{dI}{dt}$:
$$\frac{dI(t)}{dt} = C \frac{d^2V_C(t)}{dt^2}$$

### Step C: The Final Differential Equation
Substitute these expressions for $I(t)$ and $\frac{dI}{dt}$ back into **Eq. 1**:
$$L \left( C \frac{d^2V_C}{dt^2} \right) + R \left( C \frac{dV_C}{dt} \right) + V_C = V(t)$$

Rewriting in standard second-order form:
$$LC \frac{d^2V_C(t)}{dt^2} + RC \frac{dV_C(t)}{dt} + V_C(t) = V(t)$$

---

## 3. Comparison with a Damped Harmonic Oscillator

The equation of motion for a mass ($m$) on a spring with a damping coefficient ($b$), spring constant ($k$), and external force ($F$) is:
$$m \frac{d^2x}{dt^2} + b \frac{dx}{dt} + kx = F(t)$$

If we look at the RLC equation in terms of charge ($q$)—where $V_C = q/C$—the comparison becomes even clearer:
$$L \frac{d^2q}{dt^2} + R \frac{dq}{dt} + \frac{1}{C} q = V(t)$$

---

## 4. Physical Analogies

The mathematical structure of these two equations is identical, meaning the behavior of the "charge" in the circuit mimics the "position" of the mass.

| Electrical Component / Term | Mechanical Analogy | Physical Meaning |
| :--- | :--- | :--- |
| **Inductance ($L$)** | **Mass ($m$)** | Inertia (Resistance to change in motion/current) |
| **Resistance ($R$)** | **Damping ($b$)** | Dissipation (Energy lost to heat/friction) |
| **Capacitance ($1/C$)** | **Spring Constant ($k$)** | Stiffness (Restoring force/potential) |
| **Charge ($q$) or $V_C$** | **Position ($x$)** | The state variable being measured |
| **Current ($I$)** | **Velocity ($v$)** | The rate of change of the state variable |
| **Voltage Source ($V$)** | **Driving Force ($F$)** | The external input driving the system |

**Conclusion for the Teacher:** The inductor acts like mass because it "wants" to keep the current constant. The resistor acts like friction because it bleeds energy out of the system. The capacitor acts like a spring because it stores potential energy. This is why an RLC circuit can "ring" or oscillate just like a physical tuning fork.