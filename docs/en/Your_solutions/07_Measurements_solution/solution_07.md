## 7. Standard Deviation

### Problem Statement
Eleven students received the following scores on a test: 88, 92, 79, 85, 95, 81, 86, 90, 83, 77, 89. What is the mean $\bar{x} = \frac{1}{N} \sum_{i=1}^{N} x_i$ and standard deviation $\sigma = \sqrt{\frac{1}{N-1} \sum_{i=1}^{N} (x_i - \bar{x})^2}$ of these test scores? If the highest and lowest scores are removed, what are the new mean and standard deviation of the remaining scores?

---

### Solution

#### Part 1: Initial Mean and Standard Deviation

**1. Given Data ($N = 11$)**
Scores: $88, 92, 79, 85, 95, 81, 86, 90, 83, 77, 89$

**2. Calculating the Initial Mean ($\bar{x}_1$)**
First, find the sum of all scores:
$$\sum x_i = 88 + 92 + 79 + 85 + 95 + 81 + 86 + 90 + 83 + 77 + 89 = 945$$
$$\bar{x}_1 = \frac{945}{11} \approx 85.91$$

**3. Calculating the Initial Standard Deviation ($\sigma_1$)**
We use the provided formula. Let's calculate the sum of squared differences from the mean, $\sum (x_i - \bar{x})^2$:
* $(88 - 85.91)^2 \approx 4.37$
* $(92 - 85.91)^2 \approx 37.09$
* $(79 - 85.91)^2 \approx 47.75$
* $(85 - 85.91)^2 \approx 0.83$
* $(95 - 85.91)^2 \approx 82.63$
* $(81 - 85.91)^2 \approx 24.11$
* $(86 - 85.91)^2 \approx 0.01$
* $(90 - 85.91)^2 \approx 16.73$
* $(83 - 85.91)^2 \approx 8.47$
* $(77 - 85.91)^2 \approx 79.39$
* $(89 - 85.91)^2 \approx 9.55$

Sum of squared deviations $\approx 310.91$

Now, divide by $N-1$ (which is $11 - 1 = 10$) and take the square root:
$$\sigma_1 = \sqrt{\frac{310.91}{10}} = \sqrt{31.091} \approx 5.58$$

> **Important Detail on Notation:** The problem uses the symbol $\sigma$ (sigma) but provides the formula for the *sample* standard deviation (dividing by $N-1$ instead of $N$). Strictly speaking in statistics, $\sigma$ denotes *population* standard deviation (dividing by $N$), while $s$ denotes sample standard deviation. We will follow the explicit formula provided in the prompt, utilizing $N-1$ (Bessel's correction), as these 11 students are likely being treated as a sample of a larger population.

---

#### Part 2: Removing the Highest and Lowest Scores

**1. Adjusting the Data ($N = 9$)**
* **Highest score removed:** 95
* **Lowest score removed:** 77
* **Remaining Scores:** $88, 92, 79, 85, 81, 86, 90, 83, 89$

**2. Calculating the New Mean ($\bar{x}_2$)**
New Sum $= 945 - 95 - 77 = 773$
$$\bar{x}_2 = \frac{773}{9} \approx 85.89$$

**3. Calculating the New Standard Deviation ($\sigma_2$)**
Let's find the new sum of squared differences using the new mean (85.89):
* $(88 - 85.89)^2 \approx 4.45$
* $(92 - 85.89)^2 \approx 37.33$
* $(79 - 85.89)^2 \approx 47.47$
* $(85 - 85.89)^2 \approx 0.79$
* $(81 - 85.89)^2 \approx 23.91$
* $(86 - 85.89)^2 \approx 0.01$
* $(90 - 85.89)^2 \approx 16.89$
* $(83 - 85.89)^2 \approx 8.35$
* $(89 - 85.89)^2 \approx 9.67$

New sum of squared deviations $\approx 148.89$

Divide by $N-1$ (which is $9 - 1 = 8$) and take the square root:
$$\sigma_2 = \sqrt{\frac{148.89}{8}} = \sqrt{18.61} \approx 4.31$$

*Detail Note:* Notice how removing the outliers (the extreme highest and lowest values) barely changed the mean (from 85.91 to 85.89) but significantly reduced the standard deviation (from 5.58 to 4.31), demonstrating that variance is highly sensitive to extreme values!

---

### Final Answer
* **Initial Mean:** 85.91
* **Initial Standard Deviation:** 5.58
* **New Mean (outliers removed):** 85.89
* **New Standard Deviation (outliers removed):** 4.31