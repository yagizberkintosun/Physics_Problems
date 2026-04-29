# Physics Problem: Ampere's Law (Parallel Wires)

## Problem Statement
Two long, parallel wires are $10 \text{ cm}$ apart and carry currents of $5 \text{ A}$ in opposite directions. Calculate the magnitude and direction of the magnetic field at a point midway between the wires.

---

## 1. Given Data
*   **Current ($I_1 = I_2$):** $5.0 \text{ A}$
*   **Separation distance ($d$):** $10 \text{ cm} = 0.1 \text{ m}$
*   **Midway distance ($r$):** $r = \frac{d}{2} = 0.05 \text{ m}$
*   **Permeability constant ($\mu_0$):** $4\pi \times 10^{-7} \text{ T} \cdot \text{m/A}$

## 2. Physical Principles
The magnetic field $B$ produced by a single long straight wire is derived from **Ampere's Law**:
$$B = \frac{\mu_0 I}{2\pi r}$$

According to the **Principle of Superposition**, the net magnetic field $\vec{B}_{net}$ is the vector sum:
$$\vec{B}_{net} = \vec{B}_1 + \vec{B}_2$$

## 3. Direction Analysis (Right-Hand Rule)
To determine if the fields add or subtract, we apply the **Right-Hand Rule**:
*   **Wire 1 (Current Up):** At the midway point (to the right of Wire 1), the thumb points up, and fingers curl "into the page" ($\otimes$).
*   **Wire 2 (Current Down):** At the midway point (to the left of Wire 2), the thumb points down, and fingers also curl "into the page" ($\otimes$).
*   **Conclusion:** Since both vectors point in the same direction, their magnitudes add together.

## 4. Step-by-Step Calculation

**Step 1: Calculate the field from one wire ($B_1$)**
$$B_1 = \frac{(4\pi \times 10^{-7} \text{ T} \cdot \text{m/A}) \cdot (5 \text{ A})}{2\pi \cdot (0.05 \text{ m})}$$

**Step 2: Simplify the constants**
By canceling $2\pi$ from the numerator and denominator:
$$B_1 = \frac{2 \times 10^{-7} \cdot 5}{0.05}$$
$$B_1 = \frac{10 \times 10^{-7}}{0.05} = 20 \times 10^{-6} \text{ T}$$
$$B_1 = 2.0 \times 10^{-5} \text{ T}$$

**Step 3: Calculate the Net Field**
Since $I_1 = I_2$ and both wires are at the same distance $r$:
$$B_{net} = B_1 + B_2$$
$$B_{net} = 2.0 \times 10^{-5} \text{ T} + 2.0 \times 10^{-5} \text{ T}$$
$$B_{net} = 4.0 \times 10^{-5} \text{ T}$$

## 5. Final Result
The total magnetic field at the midway point is:

$$\mathbf{B_{net} = 4.0 \times 10^{-5} \text{ T (or } 40\ \mu\text{T)}}$$

**Direction:** The field is directed perpendicular to the plane of the wires (directed "into the page" based on the RHR analysis).