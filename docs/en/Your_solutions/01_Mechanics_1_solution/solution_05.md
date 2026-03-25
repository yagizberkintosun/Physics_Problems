# Relative Velocity: River Crossing Analysis

This document calculates the required heading angle and the time taken for a boat to cross a river directly north, accounting for a constant eastward current.

---

## 1. Given Parameters
* **River Velocity ($v_r$):** 2 m/s [East]
* **Boat Speed in Still Water ($v_b$):** 5 m/s
* **River Width ($d$):** 200 m
* **Desired Resultant Direction:** Directly North

---

## 2. Determining the Heading Angle ($\theta$)

To move directly north relative to the ground, the boat must head at an angle $\theta$ **West of North** so that its westward velocity component cancels out the river's eastward current.

Using the velocity vector triangle:
* The hypotenuse is the boat's speed in still water ($5$ m/s).
* The opposite side to $\theta$ is the river's speed ($2$ m/s).

$$\sin \theta = \frac{\text{Opposite}}{\text{Hypotenuse}} = \frac{v_r}{v_b}$$
$$\sin \theta = \frac{2}{5} = 0.4$$

**Solving for $\theta$:**
$$\theta = \arcsin(0.4) \approx 23.58^\circ$$

**Result:** The boat must head **23.58° West of North**.

---

## 3. Calculating the Time to Cross

First, we find the magnitude of the resultant velocity ($v_{res}$) directed North. Using the Pythagorean theorem:

$$v_{res} = \sqrt{v_b^2 - v_r^2}$$
$$v_{res} = \sqrt{5^2 - 2^2} = \sqrt{25 - 4} = \sqrt{21}$$
$$v_{res} \approx 4.583 \text{ m/s}$$

The time $t$ required to cross the width $d$ is:
$$t = \frac{d}{v_{res}}$$
$$t = \frac{200}{\sqrt{21}} \approx 43.64 \text{ s}$$

---

## Summary Table

| Parameter | Result |
| :--- | :--- |
| **Heading Angle** | 23.58° West of North |
| **Velocity Relative to Ground** | $\approx$ 4.58 m/s [North] |
| **Crossing Time** | $\approx$ 43.64 seconds |