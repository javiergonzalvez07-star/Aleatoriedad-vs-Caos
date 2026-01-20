# Random vs Chaos: Numerical Simulations in Python

This project explores the difference between **random processes** and **chaotic deterministic systems** through simple numerical simulations.  
Although random and chaotic signals may look similar at first glance, their underlying nature is fundamentally different.

The goal of this project is to show that **chaos is not randomness**: chaotic systems are deterministic and reproducible, but extremely sensitive to initial conditions.

---

## Project Overview

Several systems are studied and compared:

- **Random sequence**
  - Purely stochastic behavior
  - Non-reproducible without fixing a random seed

- **Deterministic periodic system**
  - A simple sinusoidal signal used as a non-chaotic deterministic reference

- **Logistic map**
  - A classic example of a chaotic discrete dynamical system
  - Deterministic but highly sensitive to initial conditions

- **Double pendulum**
  - A continuous-time chaotic mechanical system
  - Simulated numerically using the Runge–Kutta method

These systems are analyzed using time series, trajectory plots, and reproducibility tests.

---

## Key Concepts Illustrated

- Difference between **randomness and determinism**
- **Reproducibility** of deterministic systems
- **Sensitivity to initial conditions** as a defining feature of chaos
- Why chaotic systems can appear random despite being governed by exact equations

---

## Numerical Methods

- Time integration is performed using the **Runge–Kutta method of fourth order (RK4)**.
- The method provides stable and accurate integration without introducing randomness into the dynamics.

---

## Tools Used

- Python  
- NumPy  
- Matplotlib  
- Jupyter Notebook

---

## Structure

- `simulaciones.ipynb`  
  Main notebook containing:
  - simulations
  - visualizations
  - explanations
  - conclusions

---

## Conclusions

The simulations show that:
- Random systems are not reproducible unless a seed is fixed.
- Chaotic systems are fully deterministic and reproducible with the same initial conditions.
- Small differences in initial conditions lead to drastically different outcomes in chaotic systems.

Therefore, chaos should not be confused with randomness: it arises from deterministic rules combined with strong sensitivity to initial conditions.

---

## Author

Personal project developed as part of self-study in applied mathematics, physics, and scientific programming.

