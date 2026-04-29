# Physics Problem: Energy Stored in a Capacitor

## Problem Statement
We have a parallel-plate capacitor with the following parameters:
*   Area ($S$): $0.02 \text{ m}^2$
*   Plate separation ($d$): $5 \text{ mm}$
*   Voltage ($U$): $500 \text{ V}$

Calculate the capacitance $C$, the stored energy, the electric field intensity $E$, and the force of attraction $F$ between the plates.

---

## 1. Given Data
*   **Plate Area ($S$):** $0.02 \text{ m}^2$
*   **Separation ($d$):** $5 \text{ mm} = 0.005 \text{ m} = 5 \times 10^{-3} \text{ m}$
*   **Potential Difference ($U$):** $500 \text{ V}$
*   **Permittivity of Free Space ($\epsilon_0$):** $8.854 \times 10^{-12} \text{ F/m}$

## 2. Physical Principles
*   **Capacitance ($C$):** For a parallel-plate capacitor: $C = \frac{\epsilon_0 S}{d}$.
*   **Stored Energy ($U_{stored}$):** $U_{stored} = \frac{1}{2} C U^2$.
*   **Electric Field ($E$):** The uniform field between plates is: $E = \frac{U}{d}$.
*   **Force ($F$):** The force of attraction between plates is: $F = \frac{1}{2} Q E$ or $F = \frac{\epsilon_0 S U^2}{2 d^2}$.

## 3. Step-by-Step Calculation

### Part A: Capacitance ($C$)
$$C = \epsilon_0 \frac{S}{d}$$
$$C = (8.854 \times 10^{-12} \text{ F/m}) \cdot \frac{0.02 \text{ m}^2}{0.005 \text{ m}}$$
$$C = 8.854 \times 10^{-12} \cdot 4$$
$$C = 3.5416 \times 10^{-11} \text{ F}$$
**Result:** $C \approx 35.4 \text{ pF}$

---

### Part B: Energy Stored ($U_{stored}$)
$$U_{stored} = \frac{1}{2} C U^2$$
$$U_{stored} = 0.5 \cdot (3.5416 \times 10^{-11} \text{ F}) \cdot (500 \text{ V})^2$$
$$U_{stored} = 0.5 \cdot (3.5416 \times 10^{-11}) \cdot (250,000)$$
$$U_{stored} = 4.427 \times 10^{-6} \text{ J}$$
**Result:** $U_{stored} \approx 4.43\ \mu\text{J}$

---

### Part C: Electric Field Intensity ($E$)
$$E = \frac{U}{d}$$
$$E = \frac{500 \text{ V}}{0.005 \text{ m}}$$
$$E = 100,000 \text{ V/m}$$
**Result:** $E = 10^5 \text{ V/m}$ (or $100 \text{ kV/m}$)

---

### Part D: Force of Attraction ($F$)
The force on one plate is due to the electric field of the other. First, find the charge $Q$:
$$Q = C \cdot U = (3.5416 \times 10^{-11} \text{ F}) \cdot (500 \text{ V}) = 1.7708 \times 10^{-8} \text{ C}$$

Now, calculate the force:
$$F = \frac{1}{2} Q E$$
$$F = 0.5 \cdot (1.7708 \times 10^{-8} \text{ C}) \cdot (10^5 \text{ V/m})$$
$$F = 0.8854 \times 10^{-3} \text{ N}$$
**Result:** $F \approx 0.885 \text{ mN}$

---

## 4. Final Results Summary
| Parameter | Value |
| :--- | :--- |
| **Capacitance ($C$)** | $35.4 \text{ pF}$ |
| **Stored Energy** | $4.43\ \mu\text{J}$ |
| **Electric Field ($E$)** | $10^5 \text{ V/m}$ |
| **Force ($F$)** | $0.885 \text{ mN}$ |