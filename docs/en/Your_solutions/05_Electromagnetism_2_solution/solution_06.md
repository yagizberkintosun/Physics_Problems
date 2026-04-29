# Physics Problem: EM Wave Analysis

## Problem Statement
An electromagnetic wave has its electric field component described by:
$$E_y(x, t) = 100 \sin(10^7 x - \omega t) \text{ V/m}$$

Calculate:
1. The direction of propagation.
2. The wavelength ($\lambda$).
3. The angular frequency ($\omega$).
4. The equation for the magnetic field component ($B$).

---

## 1. Given Data and Standard Form
The given equation is in the standard form of a plane wave:
$$E_y(x, t) = E_0 \sin(kx - \omega t)$$

From comparison, we identify:
*   **Electric Field Amplitude ($E_0$):** $100 \text{ V/m}$
*   **Wave Number ($k$):** $10^7 \text{ rad/m}$
*   **Speed of Light ($c$):** $3 \times 10^8 \text{ m/s}$ (constant in vacuum)

---

## 2. Step-by-Step Analysis

### Part A: Direction of Propagation
The direction is determined by the argument of the sine function $(kx - \omega t)$:
*   The variable $x$ indicates the wave travels along the **x-axis**.
*   The negative sign between the $kx$ and $\omega t$ terms indicates the wave is moving in the **positive direction**.
*   **Result:** The wave propagates in the **$+x$ direction**.

---

### Part B: Calculation of Wavelength ($\lambda$)
The relationship between the wave number $k$ and wavelength $\lambda$ is:
$$k = \frac{2\pi}{\lambda} \implies \lambda = \frac{2\pi}{k}$$

**Calculation:**
$$\lambda = \frac{2\pi}{10^7 \text{ m}^{-1}}$$
$$\lambda = 2\pi \times 10^{-7} \text{ m}$$
$$\lambda \approx 6.28 \times 10^{-7} \text{ m} \text{ (or } 628 \text{ nm)}$$

---

### Part C: Calculation of Angular Frequency ($\omega$)
For an EM wave in a vacuum, the angular frequency is related to the wave number by the speed of light:
$$\omega = c \cdot k$$

**Calculation:**
$$\omega = (3 \times 10^8 \text{ m/s}) \cdot (10^7 \text{ rad/m})$$
$$\omega = 3 \times 10^{15} \text{ rad/s}$$

---

### Part D: Equation for the Magnetic Field Component
To write the equation for $B$, we need the amplitude and the direction.

**1. Amplitude ($B_0$):**
In an EM wave, the ratio of $E$ to $B$ is the speed of light:
$$B_0 = \frac{E_0}{c} = \frac{100 \text{ V/m}}{3 \times 10^8 \text{ m/s}}$$
$$B_0 \approx 3.33 \times 10^{-7} \text{ T}$$

**2. Direction and Phase:**
*   The magnetic field $\vec{B}$ is perpendicular to both the electric field $\vec{E}$ and the direction of propagation.
*   Direction of Propagation ($\hat{i}$) = $\hat{E} \times \hat{B}$.
*   Since $\hat{E}$ is in the $+y$ direction ($\hat{j}$), we have $\hat{j} \times \hat{B} = \hat{i}$. This implies $\hat{B}$ must be in the **+z direction** ($\hat{k}$).
*   $B$ and $E$ are in phase for a plane wave.

**Resulting Equation:**
$$B_z(x, t) = B_0 \sin(kx - \omega t)$$
$$B_z(x, t) = (3.33 \times 10^{-7}) \sin(10^7 x - 3 \times 10^{15} t) \text{ T}$$

---

## 3. Final Results Summary
*   **Direction of Propagation:** $+x$ direction
*   **Wavelength ($\lambda$):** $6.28 \times 10^{-7} \text{ m}$
*   **Angular Frequency ($\omega$):** $3 \times 10^{15} \text{ rad/s}$
*   **Magnetic Field Equation:** $B_z(x, t) = 3.33 \times 10^{-7} \sin(10^7 x - 3 \times 10^{15} t) \text{ T}$