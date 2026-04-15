# 3.Problem: Electrostatic Equilibrium of Three Point Charges

### 1. Problem Identification
We are given two fixed positive charges, $q_1 = +4\text{C}$ and $q_2 = +9\text{C}$, separated by a distance $d = 2\text{m}$. A third charge, $q_3 = +1\text{C}$, is placed between them. We need to find the specific position $x$ where $q_3$ is in **electrostatic equilibrium**.

### 2. Physical Principles
For $q_3$ to be in equilibrium, the net electrostatic force acting on it must be zero ($\sum \vec{F} = 0$). According to **Coulomb's Law**, the magnitude of the force between two point charges is given by:
$$F = k \frac{|q_a q_b|}{r^2}$$

Since $q_1$, $q_2$, and $q_3$ are all positive, $q_3$ will experience a repulsive force from both $q_1$ (pushing it to the right) and $q_2$ (pushing it to the left).

### 3. Mathematical Setup
Let $x$ be the distance from $q_1$ to $q_3$. Therefore, the distance from $q_3$ to $q_2$ must be $(2 - x)$.

At equilibrium:
$$F_{13} = F_{23}$$

Substituting the Coulomb's Law expressions:
$$k \frac{q_1 q_3}{x^2} = k \frac{q_2 q_3}{(2 - x)^2}$$

### 4. Step-by-Step Derivation
First, we can simplify the equation by canceling the electrostatic constant ($k$) and the magnitude of the test charge ($q_3$):
$$\frac{q_1}{x^2} = \frac{q_2}{(2 - x)^2}$$

Now, substitute the given values $q_1 = 4\text{C}$ and $q_2 = 9\text{C}$:
$$\frac{4}{x^2} = \frac{9}{(2 - x)^2}$$

To solve for $x$ efficiently without a complex quadratic, we take the square root of both sides:
$$\sqrt{\frac{4}{x^2}} = \sqrt{\frac{9}{(2 - x)^2}}$$
$$\frac{2}{x} = \frac{3}{2 - x}$$

### 5. Final Calculation
Cross-multiply to solve for $x$:
$$2(2 - x) = 3x$$
$$4 - 2x = 3x$$
$$4 = 5x$$
$$x = \frac{4}{5} = 0.8\text{m}$$

**Result:** The equilibrium position for $q_3$ is **$0.8\text{m}$** away from the $+4\text{C}$ charge (or $1.2\text{m}$ away from the $+9\text{C}$ charge).