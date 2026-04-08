## 10. Animation: Wave Sources

#### **1. The Physics of the Animation**
The goal of this simulation is to model the superposition (interference) of multiple 2D wave sources. The wave from each point source is described by the equation:
$$u(\vec{r}, t) = \frac{A}{|\vec{r} - \vec{r}_0|^\alpha} \sin(k|\vec{r} - \vec{r}_0| - \omega t)$$

* **$\vec{r}_0$**: The position of the wave source (where the user clicks).
* **$\vec{r}$**: The position of any given point on the screen.
* **$|\vec{r} - \vec{r}_0|$**: The physical distance ($d$) from the source to the point.
* **$\alpha$**: The attenuation parameter. When $\alpha = 0$, the wave doesn't lose energy as it travels. When $\alpha > 0$, the amplitude decays with distance.

#### **2. Superposition Principle**
To find the total wave displacement at any pixel on the screen, we apply the Principle of Superposition. We calculate $u(\vec{r}, t)$ for every individual dot, and sum them all together. The resulting positive and negative values are mapped to colors (brightness) to create the visual interference pattern.

*(Note: The actual interactive animation is contained in the accompanying HTML file).*