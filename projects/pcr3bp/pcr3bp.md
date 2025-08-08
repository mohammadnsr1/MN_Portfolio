title: PCR3BP
permalink: /projects/pcr3bp/pcr3bp
---

<link rel="stylesheet" href="/assets/css/style.css">

# Planar Circular Restricted Three‑Body Problem (PCR3BP)

![Hero](/assets/images/PCR3BD.png)

**Summary.** Derived equations in the rotating and inertial frame, Located Lagrange Points,  obtained Jacobi constant levels, and simulated sample trajectories.

## 1.	Introduction:
   In situations where two significant bodies are in circular motion around a common center of mass and a third body's mass is not significant enough to affect the other two bodies' motion, the problem of the third body's motion is referred to as the circular restricted three-body problem (CR3BP). By further restricting the motion of the third body to the same orbital plane as the other two bodies, we get the planar circular restricted three-body problem (PCR3BP).
  The planar circular restricted three-body problem (PCR3BP) is a suitable initial model for studying astronomical events such as the resonance transition of Jupiter comets, as highlighted by Koon, Lo, Marsden, and Ross [2000]. These comets are primarily heliocentric, with the sun's gravitational force being the primary factor influencing their movement, but Jupiter's gravitation causes significant perturbations from their pure two-body motion around the sun. Additionally, the comets' motion is almost entirely in Jupiter's orbital plane, and Jupiter's near-circular orbit (with low eccentricity) has little impact during resonant transitions. More importantly, the study of PCR3BP provides a systematic method for the numerical construction of initial pieces from which the final trajectory in the N-body field can be generated.


## 2.	Equations of Motion:
Let X-Y -Z be an inertial frame and x-y-z be rotating frame with origin at the m1- m2 center of mass, as in Figure 1, where the X-Y plane is the orbital plane of the primaries. Figure 2 shows the whole system with position vectors of particle with respect to the origin and massive bodies. 

First, we write the position of particle P in terms of rotating frame components (B= (G,(b1) ̂, (b2) ̂  ,(b3) ̂)), and then we compute the secondary mass (particle P) inertial velocity and acceleration with transport theorem. 
{█(r_(p/o)= x (b1) ̂  + y  (b2) ̂@r_(m1\/o)  = x1  (b1) ̂   @r_(m2/o)= x2  (b1) ̂  )┤  		                               {█(〖 V〗_(p/o)= B_d/dt  r_(p/o)  +w (e3) ̂  × r_(p/o)@〖V_(p/o)〗_ =((x ) ̇- ωy) (b1) ̂  + ( (y ) ̇+ ωx) (b2) ̂ )┤
						
{█(〖 a〗_(p/o)= B_d/dt  V_(p/o)  +w (e3) ̂  × V_(p/o)@〖a_(p/o)〗_ =(x ̈-2ωy ̇-〖 ω〗^2 x) (b1) ̂  + (y ̈+2ωx ̇-〖 ω〗^2 y) (b2) ̂ )┤


## Results
- Plots: zero‑velocity curves, trajectories near \(L_4\)/\(L_1\), inertial vs rotating
- Stability comments for \(L_4/L_5\) vs collinear points

## Notes & Future Work
- Invariant manifolds around \(L_1/L_2\)
- Halo orbits and continuation methods
