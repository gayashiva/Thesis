202111291447

**Status:** #include

**Tags:** #paper1

# [[Ice Radius evolution]]

$$
\begin{aligned}
\Delta A &= \pi * (2 * r * \Delta y + \Delta y ^2) \\
\Delta V &= 2 * \pi * r * \Delta y *\Delta z \\
\Delta M &= \Delta V * \rho_{water/ice} \\
EB &= \Delta M * L_{f}/\Delta t  \\
\Delta y^2 &= |EB|/(2 * \pi * L_{f} * \rho_{water/ice} / \Delta t *r) \\
r_i &= r_{i-1} + \Delta y \\
\end{aligned}
$$

Assumptions $\Delta y ^ 3 = 0$ , $\Delta z = \Delta y$ , $EB = Q_{freeze/melt}$
Difference in fountain on and off step

Calculated radius evolution from camera(rad_cam.py) but fountain height change varies radius unpredictably due to wind. Another possibility is that fountain aperture is also changed when fountain height is varied. Without faintain height variation, radius evolution is possible to be modelled. 

---
# References