## 9. Vertical Throw with Drag

### **1. Analytical Solution**

#### **Solving for Velocity ($v(t)$)**
Rearrange the equation:
$$\frac{dv}{dt} = -\left(g + \frac{k}{m}v\right)$$
Separate variables:
$$\frac{dv}{g + \frac{k}{m}v} = -dt$$
Integrate both sides:
$$\frac{m}{k} \ln\left(g + \frac{k}{m}v\right) = -t + C$$
Using $v(0) = v_0$, we find $C = \frac{m}{k} \ln(g + \frac{k}{m}v_0)$.
The final velocity equation is:
**$$v(t) = \left(v_0 + \frac{mg}{k}\right)e^{-\frac{k}{m}t} - \frac{mg}{k}$$**

#### **Solving for Position ($x(t)$)**
Integrate $v(t)$ with respect to $t$:
$$x(t) = \int \left[\left(v_0 + \frac{mg}{k}\right)e^{-\frac{k}{m}t} - \frac{mg}{k}\right] dt$$
$$x(t) = -\frac{m}{k}\left(v_0 + \frac{mg}{k}\right)e^{-\frac{k}{m}t} - \frac{mg}{k}t + C_2$$
Using $x(0) = 10$:
**$$x(t) = 10 + \frac{m}{k}\left(v_0 + \frac{mg}{k}\right)\left(1 - e^{-\frac{k}{m}t}\right) - \frac{mg}{k}t$$**

---

### **2. Maximum Height**
The maximum height occurs when $v(t) = 0$.
$$0 = \left(v_0 + \frac{mg}{k}\right)e^{-\frac{k}{m}t_{max}} - \frac{mg}{k}$$
Solving for $t_{max}$:
$$t_{max} = \frac{m}{k} \ln\left(1 + \frac{kv_0}{mg}\right)$$
Substitute $t_{max}$ into $x(t)$ to find $x_{max}$.

---

### **3. Comparison with Vacuum Case**
In a vacuum ($k=0$):
* $v(t) = v_0 - gt$
* $x_{max} = 10 + \frac{v_0^2}{2g}$

**Conclusion:** Air resistance (drag) reduces both the time to reach the peak and the maximum height reached.

