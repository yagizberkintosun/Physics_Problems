## 11. Animation: Two-Slit Interference (Young's Experiment)

#### **1. The Physics of the Double Slit**
This simulation models Thomas Young's famous double-slit experiment. When a coherent wave source (like a laser) passes through two narrowly spaced slits, the slits act as two new, independent point sources. As the waves propagate outward, they overlap and interfere with each other, creating a distinct pattern of alternating bright (constructive interference) and dark (destructive interference) bands.

#### **2. The Superposition Formula**
To determine the wave displacement $u$ at any given point in space ($\vec{r}$) at a specific time ($t$), we use the principle of superposition to add the partial waves from Slit 1 ($\vec{r}_1$) and Slit 2 ($\vec{r}_2$):

$$u(\vec{r}, t) = \frac{A}{|\vec{r} - \vec{r}_1|} \sin(k|\vec{r} - \vec{r}_1| - \omega t) + \frac{A}{|\vec{r} - \vec{r}_2|} \sin(k|\vec{r} - \vec{r}_2| - \omega t)$$

**Key Variables in the Simulation:**
* **$d$ (Distance between slits):** Calculated as $|\vec{r}_1 - \vec{r}_2|$. Moving the slits closer together or further apart dramatically changes the angles of the interference fringes.
* **$\lambda$ (Wavelength):** Determines the wave number ($k = \frac{2\pi}{\lambda}$). Longer wavelengths create wider, more spread-out interference patterns.
* The $1/|\vec{r} - \vec{r}_n|$ term ensures the amplitude naturally decays as the wave travels further from the slit, accurately representing the conservation of energy in 2D space.

*(Note: The interactive simulation allows real-time adjustment of $d$ and $\lambda$. See the accompanying HTML file for the rendering engine).*