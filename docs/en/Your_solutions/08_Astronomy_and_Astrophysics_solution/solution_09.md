## Problem 9: Size and Distance of the Sun

### Given / Knowns
* Earth-Moon-Sun angle at the Moon (dichotomy), $\angle M = 90^\circ$
* Angular separation between Sun and Moon from Earth, $\theta = 89.85^\circ$
* Apparent angular diameter of Sun and Moon, $\alpha = 0.53^\circ$
* Average Earth-Moon distance, $d_{EM} = 3.84 \times 10^5 \text{ km}$

### Concepts & Assumptions
* **Right Triangle Trigonometry:** At the exact half-moon, the Earth, Moon, and Sun form a right-angled triangle. We can use the cosine function relating the adjacent side (Earth-Moon distance) to the hypotenuse (Earth-Sun distance).
* **Small-Angle Approximation:** For very small angles, the tangent or sine of the angle is approximately equal to the angle itself (when measured in radians). This allows us to relate the physical diameter of a distant object to its distance and apparent angular size: $\alpha \approx D / d$.
* **Identical Angular Sizes:** Because solar eclipses occur where the Moon perfectly covers the Sun, both bodies have the same apparent angular size ($\alpha$) from Earth, meaning their physical diameters scale directly with their distances.

### Formulas
* Trigonometric Relation: $\cos(\theta) = \frac{\text{Adjacent}}{\text{Hypotenuse}} = \frac{d_{EM}}{d_{ES}}$
* Degrees to Radians: $\text{Radians} = \text{Degrees} \times \left(\frac{\pi}{180}\right)$
* Small-Angle Approximation: $\alpha \approx \frac{D}{d} \implies D \approx \alpha d$

---

### Step-by-Step Derivation

#### 1. The Earth-Sun distance $d_{ES}$
Using the right triangle formed by the Earth, Moon, and Sun, where the right angle is at the Moon:

$$\cos(\theta) = \frac{d_{EM}}{d_{ES}}$$

Rearrange to solve for the Earth-Sun distance ($d_{ES}$):

$$d_{ES} = \frac{d_{EM}}{\cos(\theta)}$$

$$d_{ES} = \frac{3.84 \times 10^5 \text{ km}}{\cos(89.85^\circ)}$$

$$d_{ES} = \frac{3.84 \times 10^5 \text{ km}}{0.002618}$$

$$d_{ES} \approx 146,677,205 \text{ km} \approx 1.467 \times 10^8 \text{ km}$$

#### 2. The true diameter of the Sun $D_S$
First, convert the angular diameter $\alpha$ from degrees to radians:

$$\alpha = 0.53^\circ \times \left(\frac{\pi}{180}\right)$$

$$\alpha \approx 0.00925 \text{ rad}$$

Now apply the small-angle approximation:

$$D_S = \alpha \times d_{ES}$$

$$D_S = 0.00925 \text{ rad} \times 146,677,205 \text{ km}$$

$$D_S \approx 1,356,764 \text{ km} \approx 1.357 \times 10^6 \text{ km}$$

#### 3. The ratio of true diameters $D_M / D_S$
Since both the Sun and the Moon have the same apparent angular diameter ($\alpha$), we can set up the following relationships:

$$\alpha = \frac{D_M}{d_{EM}} \quad \text{and} \quad \alpha = \frac{D_S}{d_{ES}}$$

Set them equal to each other:

$$\frac{D_M}{d_{EM}} = \frac{D_S}{d_{ES}}$$

Rearrange to find the ratio of their diameters:

$$\frac{D_M}{D_S} = \frac{d_{EM}}{d_{ES}}$$

Notice that $\frac{d_{EM}}{d_{ES}}$ is exactly the cosine of $\theta$ that we started with!

$$\frac{D_M}{D_S} = \cos(89.85^\circ)$$

$$\frac{D_M}{D_S} \approx 0.002618$$

*(Note: This means the Moon's diameter is roughly 1/382 of the Sun's diameter).*

#### 4. Sensitivity of the result if $\theta = 89.75^\circ$

Recalculate $d_{ES}$ using the new angle:

$$d_{ES}' = \frac{d_{EM}}{\cos(89.75^\circ)}$$

$$d_{ES}' = \frac{3.84 \times 10^5 \text{ km}}{0.004363}$$

$$d_{ES}' \approx 88,006,600 \text{ km}$$

Calculate the change in distance:

$$\Delta d = d_{ES} - d_{ES}'$$

$$\Delta d = 146,677,205 \text{ km} - 88,006,600 \text{ km}$$

$$\Delta d \approx 58,670,605 \text{ km}$$

**Commentary on Sensitivity:**
A minuscule change of just **$0.1^\circ$** in the angular measurement resulted in a massive difference of nearly **58.7 million kilometers** (a roughly 40% error). This demonstrates that the cosine function is highly sensitive (its derivative is very steep) as the angle approaches $90^\circ$. For Aristarchus, this implies that while his geometric *method* was perfectly logical, his practical *results* were doomed to be highly inaccurate. It is physically impossible to judge the exact moment of a "half-moon" with the naked eye to a fraction of a degree.

---

### Final Answer
1. The Earth-Sun distance $d_{ES}$ is approximately **$1.467 \times 10^8$ km**.
2. The true diameter of the Sun $D_S$ is approximately **$1.357 \times 10^6$ km**.
3. The ratio of true diameters $\frac{D_M}{D_S}$ is **0.002618**.
4. Changing the angle by just $0.1^\circ$ reduces the calculated distance by **$5.87 \times 10^7$ km**, proving the method is incredibly sensitive to measurement error near $90^\circ$.