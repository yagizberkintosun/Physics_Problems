# Physics Problem: Series and Parallel Circuits

## 1. Problem Statement
We have three resistors with the following values:
*   $R_1 = 15\ \Omega$
*   $R_2 = 30\ \Omega$
*   $R_3 = 50\ \Omega$

The resistors are connected to a **12 V battery**. We need to determine the **total equivalent resistance** ($R_{eq}$) and the **total current** ($I_{total}$) flowing from the battery for two distinct scenarios:
1.  When all resistors are connected in **series**.
2.  When all resistors are connected in **parallel**.

---

## 2. Fundamental Physics Concepts

### Ohm's Law
The relationship between voltage ($V$), current ($I$), and resistance ($R$) is defined by Ohm's Law:
$$V = I \cdot R \implies I = \frac{V}{R}$$

### Series Circuits
In a series circuit, there is only one path for the current. The total resistance is the sum of the individual resistances:
$$R_{series} = R_1 + R_2 + R_3 + \dots + R_n$$

### Parallel Circuits
In a parallel circuit, the voltage across each resistor is the same, but the current splits. The reciprocal of the total resistance is the sum of the reciprocals of the individual resistances:
$$\frac{1}{R_{parallel}} = \frac{1}{R_1} + \frac{1}{R_2} + \frac{1}{R_3} + \dots + \frac{1}{R_n}$$

---

## 3. Case 1: Series Connection

### Step A: Calculate Equivalent Resistance
Since the resistors are in series, we simply sum their values:
$$R_{eq(s)} = R_1 + R_2 + R_3$$
$$R_{eq(s)} = 15\ \Omega + 30\ \Omega + 50\ \Omega$$
$$R_{eq(s)} = 95\ \Omega$$

### Step B: Calculate Total Current
Using Ohm's Law with the total voltage and the series equivalent resistance:
$$I_s = \frac{V}{R_{eq(s)}}$$
$$I_s = \frac{12\ \text{V}}{95\ \Omega}$$
$$I_s \approx 0.1263\ \text{A} \text{ (or 126.3 mA)}$$

---

## 4. Case 2: Parallel Connection

### Step A: Calculate Equivalent Resistance
For parallel resistors, we use the reciprocal formula:
$$\frac{1}{R_{eq(p)}} = \frac{1}{R_1} + \frac{1}{R_2} + \frac{1}{R_3}$$
$$\frac{1}{R_{eq(p)}} = \frac{1}{15} + \frac{1}{30} + \frac{1}{50}$$

To solve this, we find a common denominator (150):
$$\frac{1}{R_{eq(p)}} = \frac{10}{150} + \frac{5}{150} + \frac{3}{150} = \frac{18}{150}$$

Now, take the reciprocal to find $R_{eq(p)}$:
$$R_{eq(p)} = \frac{150}{18}\ \Omega \approx 8.33\ \Omega$$

### Step B: Calculate Total Current
Using Ohm's Law with the parallel equivalent resistance:
$$I_p = \frac{V}{R_{eq(p)}}$$
$$I_p = \frac{12\ \text{V}}{8.333\dots\ \Omega}$$
$$I_p = 1.44\ \text{A}$$

---

## 5. Summary of Results

| Connection Type | Total Resistance ($R_{eq}$) | Current from Battery ($I$) |
| :--- | :--- | :--- |
| **Series** | $95\ \Omega$ | $0.126\ \text{A}$ |
| **Parallel** | $8.33\ \Omega$ | $1.440\ \text{A}$ |

**Conclusion:** Note that in a parallel circuit, the total resistance is lower than the smallest individual resistor ($8.33\ \Omega < 15\ \Omega$), which results in a significantly higher current draw from the battery compared to the series configuration.