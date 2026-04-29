# Physics Problem: Biot-Savart Law

## Problem Statement
A small segment of a line wire of length $0.1 \text{ m}$ carries a current of $3 \text{ A}$. The segment is located at a distance of $0.2 \text{ m}$ from a point $P$. Calculate the magnetic field at point $P$ due to this current segment (assume the segment is perpendicular to the line connecting it to point $P$).

---

## 1. Given Data
*   **Length of the segment ($dl$):** $0.1 \text{ m}$
*   **Current ($I$):** $3 \text{ A}$
*   **Distance to point $P$ ($r$):** $0.2 \text{ m}$
*   **Orientation:** Perpendicular ($\theta = 90^\circ$)
*   **Permeability constant ($\frac{\mu_0}{4\pi}$):** $10^{-7} \text{ T} \cdot \text{m/A}$

## 2. Physical Principles
The **Biot-Savart Law** allows us to calculate the magnetic field ($dB$) produced by a small current element. The magnitude is given by:

$$dB = \frac{\mu_0}{4\pi} \frac{I \cdot dl \cdot \sin(\theta)}{r^2}$$

Where:
*   $I$ is the current.
*   $dl$ is the differential length of the wire.
*   $r$ is the distance from the segment to the point $P$.
*   $\theta$ is the angle between the current direction and the vector pointing to $P$.

## 3. Step-by-Step Calculation

**Step 1: Determine the sine of the angle**
Because the problem states the segment is perpendicular to the line connecting it to $P$:
$$\theta = 90^\circ \implies \sin(90^\circ) = 1$$

**Step 2: Substitute the known values into the formula**
Using $\frac{\mu_0}{4\pi} = 10^{-7}$:
$$B = (10^{-7} \text{ T} \cdot \text{m/A}) \cdot \frac{(3 \text{ A}) \cdot (0.1 \text{ m}) \cdot (1)}{(0.2 \text{ m})^2}$$

**Step 3: Simplify the numerator and denominator**
*   **Numerator:** $3 \cdot 0.1 \cdot 1 = 0.3 \text{ A} \cdot \text{m}$
*   **Denominator:** $(0.2)^2 = 0.04 \text{ m}^2$

$$B = 10^{-7} \cdot \frac{0.3}{0.04}$$

**Step 4: Solve for the final magnitude**
Dividing $0.3$ by $0.04$ gives $7.5$:
$$B = 7.5 \times 10^{-7} \text{ T}$$

## 4. Final Result
The magnetic field at point $P$ is:

$$\mathbf{B = 7.5 \times 10^{-7} \text{ T (or } 0.75\ \mu\text{T)}}$$