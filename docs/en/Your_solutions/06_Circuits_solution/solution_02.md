# Physics Problem: Combinations of Resistors

## 1. Problem Statement
We are given:
*   Three identical resistors, each with a resistance $R = 1\ \Omega$.
*   Goal: Determine all possible equivalent resistances ($R_{eq}$) that can be created by combining all three resistors in various circuit configurations.

---

## 2. Governing Principles

To solve this, we use the two fundamental rules for combining resistors:

1.  **Series Combination:** The total resistance is the sum of individual resistances.
    $$R_{series} = R_1 + R_2 + \dots + R_n$$
2.  **Parallel Combination:** The reciprocal of the total resistance is the sum of the reciprocals of individual resistances.
    $$\frac{1}{R_{parallel}} = \frac{1}{R_1} + \frac{1}{R_2} + \dots + \frac{1}{R_n}$$

---

## 3. Possible Configurations and Calculations

There are four unique ways to connect three identical resistors.

### Case A: All Three in Series
In this layout, the current must pass through each resistor sequentially.
*   **Formula:** $R_{eq} = R + R + R$
*   **Calculation:** $R_{eq} = 1\ \Omega + 1\ \Omega + 1\ \Omega = 3\ \Omega$
*   **Result:** $3\ \Omega$

### Case B: All Three in Parallel
In this layout, the voltage across each resistor is the same, and the current splits three ways.
*   **Formula:** $\frac{1}{R_{eq}} = \frac{1}{R} + \frac{1}{R} + \frac{1}{R}$
*   **Calculation:** $\frac{1}{R_{eq}} = \frac{1}{1} + \frac{1}{1} + \frac{1}{1} = 3$
*   **Reciprocal:** $R_{eq} = \frac{1}{3}\ \Omega$
*   **Result:** $\approx 0.33\ \Omega$

### Case C: Two in Parallel, Series with One (Mixed)
Two resistors are connected in parallel first, and that "block" is then connected in series with the third resistor.
1.  **Parallel Block ($R_p$):** $\frac{1}{R_p} = \frac{1}{1} + \frac{1}{1} = 2 \implies R_p = 0.5\ \Omega$
2.  **Total ($R_{eq}$):** $R_{eq} = R_p + R = 0.5\ \Omega + 1\ \Omega$
*   **Result:** $1.5\ \Omega$ (or $\frac{3}{2}\ \Omega$)

### Case D: Two in Series, Parallel with One (Mixed)
Two resistors are connected in series first, and that "block" is then connected in parallel with the third resistor.
1.  **Series Block ($R_s$):** $R_s = 1\ \Omega + 1\ \Omega = 2\ \Omega$
2.  **Total ($R_{eq}$):** $\frac{1}{R_{eq}} = \frac{1}{R_s} + \frac{1}{R} = \frac{1}{2} + \frac{1}{1} = \frac{3}{2}$
3.  **Reciprocal:** $R_{eq} = \frac{2}{3}\ \Omega$
*   **Result:** $\approx 0.67\ \Omega$

---

## 4. Summary of Unique Values

Combining exactly three $1\ \Omega$ resistors yields the following **four unique equivalent resistances**:

| Configuration | Fractional Value | Decimal Value |
| :--- | :--- | :--- |
| **All Series** | $3\ \Omega$ | $3.00\ \Omega$ |
| **All Parallel** | $\frac{1}{3}\ \Omega$ | $0.33\ \Omega$ |
| **Two Parallel + One Series** | $\frac{3}{2}\ \Omega$ | $1.50\ \Omega$ |
| **Two Series + One Parallel** | $\frac{2}{3}\ \Omega$ | $0.67\ \Omega$ |