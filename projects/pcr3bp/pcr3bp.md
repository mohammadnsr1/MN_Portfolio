title: PCR3BP
permalink: /projects/pcr3bp/pcr3bp
---

<link rel="stylesheet" href="/assets/css/style.css">

# Planar Circular Restricted Three‑Body Problem (PCR3BP)

![Hero](/assets/images/PCR3BD.png)

**Summary.** Derived equations in the rotating frame, located **L1–L5**, plotted **zero‑velocity curves** (Jacobi constant levels), and simulated sample trajectories.

## Problem Setup
- Non‑dimensionalization, Earth–Moon mass ratio \( \mu = 0.01215 \)
- Rotating frame with primaries at \( (-\mu, 0) \) and \( (1-\mu, 0) \)
- State vector, effective potential \( \Omega \), and equations of motion

## Methods
- Solve collinear points via root finding
- \(L_4, L_5\) from equilateral geometry
- ODE45 integration for trajectories

## Results
- Plots: zero‑velocity curves, trajectories near \(L_4\)/\(L_1\), inertial vs rotating
- Stability comments for \(L_4/L_5\) vs collinear points

## Notes & Future Work
- Invariant manifolds around \(L_1/L_2\)
- Halo orbits and continuation methods
