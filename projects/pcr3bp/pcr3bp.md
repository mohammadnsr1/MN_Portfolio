title: PCR3BP
permalink: /projects/pcr3bp/
---

<link rel="stylesheet" href="/assets/css/style.css">
<!-- Enable MathJax for LaTeX rendering -->
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async
  src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js">
</script>

# Planar Circular Restricted Three‑Body Problem (PCR3BP)

![Hero](/assets/images/PCR3BD.png)

**Summary.** Derived equations in the rotating and inertial frame, Located Lagrange Points,  obtained Jacobi constant levels, and simulated sample trajectories.

## 1.Introduction:
   In situations where two significant bodies are in circular motion around a common center of mass and a third body's mass is not significant enough to affect the other two bodies' motion, the problem of the third body's motion is referred to as the circular restricted three-body problem (CR3BP). By further restricting the motion of the third body to the same orbital plane as the other two bodies, we get the planar circular restricted three-body problem (PCR3BP).
  The planar circular restricted three-body problem (PCR3BP) is a suitable initial model for studying astronomical events such as the resonance transition of Jupiter comets, as highlighted by Koon, Lo, Marsden, and Ross [2000]. These comets are primarily heliocentric, with the sun's gravitational force being the primary factor influencing their movement, but Jupiter's gravitation causes significant perturbations from their pure two-body motion around the sun. Additionally, the comets' motion is almost entirely in Jupiter's orbital plane, and Jupiter's near-circular orbit (with low eccentricity) has little impact during resonant transitions. More importantly, the study of PCR3BP provides a systematic method for the numerical construction of initial pieces from which the final trajectory in the N-body field can be generated.


## 2.Equations of Motion:

Let \(X\!-\!Y\!-\!Z\) denote an **inertial frame**, and \(x\!-\!y\!-\!z\) a **rotating frame** whose origin is located at the **center of mass of the primaries** \(m_1\) and \(m_2\), as shown in *Figure&nbsp;1*.  
The \(X\!-\!Y\) plane coincides with the orbital plane of the primaries.

*Figure&nbsp;2* shows the entire system, including the position vectors of a particle \(P\) with respect to the origin and to each massive body.

We first express the position of particle \(P\) in terms of the rotating frame components  
\[
\mathcal{B} = \left(G, \hat{\mathbf{b}}_1, \hat{\mathbf{b}}_2, \hat{\mathbf{b}}_3 \right)
\]
and then compute the **inertial velocity** and **acceleration** of \(P\) using the **transport theorem**.

---

### Position and Velocity

$$
\begin{cases}
\mathbf{r}_{p/o} = x\,\hat{\mathbf{b}}_1 + y\,\hat{\mathbf{b}}_2 \\
\mathbf{r}_{m_1/o} = x_1\,\hat{\mathbf{b}}_1 \\
\mathbf{r}_{m_2/o} = x_2\,\hat{\mathbf{b}}_1 \\
\mathbf{V}_{p/o} = \frac{B_d}{dt}\,\mathbf{r}_{p/o} + \omega\,\hat{\mathbf{e}}_3 \times \mathbf{r}_{p/o} \\
\mathbf{V}_{p/o} = (\dot{x} - \omega y)\,\hat{\mathbf{b}}_1 + (\dot{y} + \omega x)\,\hat{\mathbf{b}}_2
\end{cases}
$$

---

### Acceleration

$$
\begin{cases}
\mathbf{a}_{p/o} = \frac{B_d}{dt}\,\mathbf{V}_{p/o} + \omega\,\hat{\mathbf{e}}_3 \times \mathbf{V}_{p/o} \\
\mathbf{a}_{p/o} = (\ddot{x} - 2\omega\dot{y} - \omega^2 x)\,\hat{\mathbf{b}}_1 +
                   (\ddot{y} + 2\omega\dot{x} - \omega^2 y)\,\hat{\mathbf{b}}_2
\end{cases}
$$. 










With acceleration obtained for the secondary mass, we are now ready to apply Newton second law to get the equations of motion. The FBD for particle is shown in Figure3. The forces acting on the secondary mass are in r1 and r2 direction. As a result, we need to express r1 and r2 in terms of B frame components. Then, we introduce two other variables as µ1 = Gm1 and µ2 = Gm2 apply Newton second law to get the equations of motion. 


## 3.Equilibrium points or Lagrange points:
Although Equations of motion have no closed form analytical solution, we can use them to determine the location of the equilibrium points. These are the locations in space where the secondary mass m would have zero velocity and zero acceleration, i.e., where m would appear permanently at rest relative to m1 and m2 (and therefore appear to an inertial observer to move in circular orbits around m1 and m2). Once placed at an equilibrium point (also called liberation point or Lagrange point), a body will presumably stay there. The equilibrium points are therefore defined by the conditions: 




Substituting conditions in equations of motion results in: 




Based on Kepler law  





Solving  (i) and (ii) using the (iii)  we can obtain that:




Solving (i),(ii) numerically with MATLAB results in 5 equilibrium points shown in Figure 4. It is worthy to note that equations have been non-dimensionalized and only depend on the reduced mass parameter. Therefore, we can compute the Lagrange points ,for every system.

## 4.Jacobi Constant:
Multiplying equations of motion by x ̇ and y ̇ we obtain: 



Summing the left- and right-hand sides we obtain: 



We also can have following relations:





Substituting (i),(ii),(iii),(iiii)   to (I) we obtain












1/2 v^2 is the kinetic energy per unit mass relative to the rotating frame. −µ1/r1 and −µ2/r2 are the gravitational potential energies of the two primary masses. −〖 ω〗^2 (x2 + y2)/2 may be interpreted as the potential energy of the centrifugal force per unit mass induced by the rotation of the reference frame. The constant C is known as the Jacobi constant. Jacobi’s constant may be interpreted as the total energy of the secondary particle relative to the rotating frame. C is a constant of the motion of the secondary mass just like the energy and angular momentum are constants of the relative motion in the two-body problem. Solving this equation for v^2 yields: 






For a given value of the Jacobi constant, v^2  is a function only of position in the rotating frame. Since v2 cannot be negative, it must be true that:





Trajectories of the secondary body in regions where this inequality is violated are not allowed. The boundaries between forbidden and allowed regions of motion are found by setting v^2=0





For a given value of the Jacobi constant the curves of zero velocity are determined by this equation. Figure 4 to Figure 11 show the results.





## 5.Results of solving equations of particle motion for different levels of energy








## 6. Conclusion:
In this project the planar circular restricted 3 body problem was studied; first we derived the equations of motion using Newtonian approach, and then we derived the equilibrium points where the secondary mass would permanently appear to be at rest relative to mass m1 and m2. Moreover, we discussed an important concept called Jacobi constant which can be interpreted as the secondary mass total energy. We understood that for a given value of Jacobi constant the secondary mass would be allowed to move in certain regions. Finally, we visualized the secondary mass motion for different levels of energy in an inertial frame and rotating frame. 

