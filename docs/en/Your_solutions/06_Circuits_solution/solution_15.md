# Physics Problem: Equivalent Resistance of a Resistor Cube

## 1. Problem Statement
A cube is constructed using 12 identical resistors, each with resistance $R$, placed along its edges. 

**Goal:** Determine the total equivalent resistance ($R_{eq}$) between two **opposite corners** of the cube (across the space diagonal).

---

## 2. Fundamental Physics Concepts

### Symmetry and Equipotential Nodes
In a perfectly symmetrical circuit, points that occupy identical positions relative to the input and output terminals will have the same electrical potential. We can "short" these equipotential nodes together without changing the behavior of the circuit, which simplifies the parallel and series calculations.

### Ohm's Law
The total equivalent resistance is defined by the ratio of the total voltage drop ($V$) to the total current ($I$):
$$R_{eq} = \frac{V}{I}$$

---

## 3. Step-by-Step Derivation using Current Distribution

To find the resistance, let's imagine a total current $I$ entering the cube at one corner (Node A) and leaving at the opposite corner (Node B).

### Step A: The First Layer (Entrance)
At Node A, the current has **three identical paths** to follow (the three edges connected to the corner). Due to symmetry, the current splits equally:
*   Current through each of the first 3 resistors = $\frac{I}{3}$
*   Voltage drop for this layer: $V_1 = \frac{I}{3} \cdot R$

### Step B: The Middle Layer
After the first set of resistors, the current reaches three intermediate nodes. From each of these nodes, there are **two paths** available to continue toward the exit. Since there are 3 nodes splitting into 2 paths each, there are 6 resistors in this middle "belt":
*   Current through each of these 6 resistors = $\frac{I/3}{2} = \frac{I}{6}$
*   Voltage drop for this layer: $V_2 = \frac{I}{6} \cdot R$

### Step C: The Third Layer (Exit)
Finally, the currents converge at three nodes before the exit corner (Node B). To leave Node B as a total current $I$, the three paths must carry equal amounts again:
*   Current through each of the last 3 resistors = $\frac{I}{3}$
*   Voltage drop for this layer: $V_3 = \frac{I}{3} \cdot R$

---

## 4. Calculating the Total Resistance

The total voltage drop $V$ across the entire cube is the sum of the voltage drops across each layer:
$$V = V_1 + V_2 + V_3$$
$$V = \left( \frac{I}{3} \cdot R \right) + \left( \frac{I}{6} \cdot R \right) + \left( \frac{I}{3} \cdot R \right)$$

To add these, we find a common denominator (6):
$$V = \left( \frac{2}{6}IR \right) + \left( \frac{1}{6}IR \right) + \left( \frac{2}{6}IR \right)$$
$$V = \frac{5}{6}IR$$

Applying the definition of equivalent resistance ($R_{eq} = V / I$):
$$R_{eq} = \frac{\frac{5}{6}IR}{I}$$
**$$R_{eq} = \frac{5}{6}R$$**

---

## 5. Summary of Result
The equivalent resistance between opposite corners of a cube made of 12 resistors of resistance $R$ is:
**$$R_{eq} = \frac{5}{6}R$$**

**Teacher's Note:** This result is only possible because of the perfect symmetry of the cube. If the resistors had different values, we would have had to use a much more laborious method involving a system of 12 simultaneous equations (Mesh or Nodal analysis).