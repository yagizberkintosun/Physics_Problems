# Physics Problem: Gauss's Law

## Problem Statement
A point charge of $+2 \text{ C}$ is located at the origin. Calculate the electric flux through a spherical surface of radius $1 \text{ m}$ centered at the origin.

---

## 1. Given Data
*   **Point Charge ($q$):** $+2 \text{ C}$
*   **Radius of Sphere ($r$):** $1 \text{ m}$
*   **Permittivity of Free Space ($\epsilon_0$):** $8.854 \times 10^{-12} \text{ C}^2/(\text{N} \cdot \text{m}^2)$

## 2. Physical Principles
The problem is solved using **Gauss's Law**, which states that the total electric flux ($\Phi_E$) through any closed surface is equal to the total enclosed net charge ($q_{enc}$) divided by the permittivity of free space ($\epsilon_0$).

The mathematical expression is:
$$\Phi_E = \oint \vec{E} \cdot d\vec{A} = \frac{q_{enc}}{\epsilon_0}$$

## 3. Conceptual Analysis
*   **Symmetry:** Since the charge is a point charge at the center of a spherical surface, the electric field is uniform in magnitude across the surface and always perpendicular to it.
*   **Independence of Radius:** According to Gauss's Law, the flux depends **only** on the amount of charge enclosed. While the radius $r = 1 \text{ m}$ defines the surface, the total number of electric field lines passing through the sphere remains the same regardless of the sphere's size, provided the charge remains enclosed.

## 4. Calculation Steps

**Step 1: Identify Enclosed Charge**
Since the sphere is centered at the origin and the charge is at the origin, the entire charge is inside the surface.
$$q_{enc} = +2 \text{ C}$$

**Step 2: Substitute into Gauss's Law**
$$\Phi_E = \frac{2 \text{ C}}{8.854 \times 10^{-12} \frac{\text{C}^2}{\text{N} \cdot \text{m}^2}}$$

**Step 3: Solve for $\Phi_E$**
$$\Phi_E \approx 2.258866 \times 10^{11} \text{ N} \cdot \text{m}^2/\text{C}$$

## 5. Final Result
Rounding to three significant figures, the total electric flux is:

$$\mathbf{\Phi_E \approx 2.26 \times 10^{11} \text{ N} \cdot \text{m}^2/\text{C}}$$