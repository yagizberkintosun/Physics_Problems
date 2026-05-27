## 10. Light Speed Measurement

### Problem Statement
Measure the speed of light using a microwave oven, a bar of chocolate (or slices of cheese), and a ruler. Measure the distance between the melted spots to determine the wavelength. Use $f = 2.45\text{ GHz}$ to calculate the speed of light. Compare it to $c = 300,000,000\text{ m/s}$ and calculate the percentage error.

---

### Solution & Manual Calculations

#### 1. Experimental Data (Sample Run)
* **Frequency of Microwave ($f$):** $2.45\text{ GHz} = 2.45 \times 10^9\text{ Hz}$
* **Accepted Speed of Light ($c_{\text{true}}$):** $300,000,000\text{ m/s}$ (or $3.00 \times 10^8\text{ m/s}$)
* **Measured Distance between melted spots ($d$):** $6.1\text{ cm} = 0.061\text{ m}$ *(Sample Data)*

> **Important Physics Context:** Microwaves form **standing waves** inside the oven chamber. The chocolate melts fastest at the "antinodes" (points of maximum amplitude/energy). The distance between two adjacent antinodes in a standing wave is exactly **half of the wavelength** ($\lambda/2$).

---

#### 2. Determining the Wavelength ($\lambda$)
Since the measured distance $d$ represents half a wavelength:
$$d = \frac{\lambda}{2} \implies \lambda = 2d$$

Substituting our sample measurement:
$$\lambda = 2 \times 0.061\text{ m} = 0.122\text{ m}$$

---

#### 3. Calculating the Measured Speed of Light ($c_{\text{exp}}$)
The universal wave equation relates speed, frequency, and wavelength:
$$v = f \cdot \lambda$$
$$c_{\text{exp}} = (2.45 \times 10^9\text{ Hz}) \cdot (0.122\text{ m})$$
$$c_{\text{exp}} = 298,900,000\text{ m/s}$$

*(In scientific notation: $c_{\text{exp}} \approx 2.99 \times 10^8\text{ m/s}$)*

---

#### 4. Calculating Percentage Error
To see how accurate our kitchen-table experiment is, we compare our experimental value to the accepted value using the standard percentage error formula:

$$\text{Percentage Error} = \left| \frac{\text{Experimental Value} - \text{Accepted Value}}{\text{Accepted Value}} \right| \times 100\%$$

$$\text{Percentage Error} = \left| \frac{298,900,000 - 300,000,000}{300,000,000} \right| \times 100\%$$

$$\text{Percentage Error} = \left| \frac{-1,100,000}{300,000,000} \right| \times 100\%$$

$$\text{Percentage Error} \approx 0.003667 \times 100\% \approx 0.37\%$$

---

### Final Result
* **Calculated Speed of Light:** $298,900,000\text{ m/s}$
* **Percentage Error:** $0.37\%$

*Conclusion: The calculated result is extremely close to the accepted value of $300,000,000\text{ m/s}$, demonstrating that measuring standing wave antinodes with chocolate is a highly effective, albeit slightly messy, method for calculating the speed of light!*