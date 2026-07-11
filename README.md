# Randomness vs Chaos: Numerical Experiments in Python

A numerical exploration of the difference between **stochastic processes** and **deterministic chaotic systems**.

Random and chaotic signals can look similar, but their underlying mechanisms are fundamentally different. This project uses reproducibility tests, time-series visualisations, the logistic map, and a double-pendulum simulation to show a central idea:

> Chaos is not randomness. A chaotic system is governed by deterministic equations, yet small differences in initial conditions can produce radically different trajectories.

## Systems studied

### Random sequence

Used as a stochastic reference:

- values are generated probabilistically;
- results are not reproducible unless the random seed is fixed;
- apparent unpredictability comes from the generation process itself.

### Periodic deterministic system

A sinusoidal signal provides a non-chaotic deterministic baseline:

- the governing rule is fixed;
- the trajectory is reproducible;
- nearby initial conditions do not diverge dramatically.

### Logistic map

The logistic map is used as a compact example of discrete chaos:

- the update rule is deterministic;
- the same initial condition produces the same sequence;
- nearby initial conditions can diverge quickly in chaotic parameter regimes.

### Double pendulum

The double pendulum provides a continuous mechanical example:

- the equations of motion are deterministic;
- trajectories are integrated numerically;
- very small changes in the starting state can lead to visibly different motion.

## Numerical method

The continuous dynamics are integrated using the **fourth-order Runge-Kutta method (RK4)**.

RK4 provides an accurate deterministic time-stepping method and makes it possible to separate numerical simulation from the concept of randomness: the apparent unpredictability comes from sensitivity to initial conditions, not from random terms in the equations.

## What the notebook demonstrates

- stochastic and deterministic signals can appear visually similar;
- fixing a random seed restores reproducibility to a random generator, but does not make the process deterministic in the physical sense;
- deterministic systems reproduce exactly when initial conditions and parameters are unchanged;
- chaotic systems amplify tiny initial differences;
- predictability can be limited even when the governing equations are known.

## Repository structure

```text
simulaciones.ipynb
```

The notebook contains the simulations, visualisations, comparisons, and conclusions.

## Technologies

- Python
- NumPy
- Matplotlib
- Jupyter Notebook
- Numerical integration with RK4

## How to run

```bash
git clone https://github.com/javiergonzalvez07-star/Aleatoriedad-vs-Caos.git
cd Aleatoriedad-vs-Caos

python -m venv .venv
python -m pip install --upgrade pip
python -m pip install numpy matplotlib jupyter
```

Open `simulaciones.ipynb` and run the cells in order.

## Limitations and next steps

The project is designed as an intuitive numerical study rather than a complete nonlinear-dynamics analysis. Future extensions could include:

- Lyapunov-exponent estimation;
- bifurcation diagrams for the logistic map;
- Poincare sections;
- phase-space reconstruction;
- quantitative divergence-rate comparisons;
- sensitivity to numerical step size.

## Author

**Javier Gonzálvez Sempere**  
Double Degree student in Mathematical Engineering and Physics.

- Portfolio: https://javiergonzalvez07-star.github.io/
- GitHub: https://github.com/javiergonzalvez07-star
