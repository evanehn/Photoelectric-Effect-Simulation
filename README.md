# Continuous Dynamics Simulation of the Photoelectric Effect

A numerical physics simulation modeling the ejection and trajectory of photoelectrons from a sodium plate ($\Phi = 2.28\text{ eV}$) inside a parallel-plate electric field. Built in Python as a final project for **EPS 109 (Computer Simulations in Earth and Planetary Sciences)** at UC Berkeley.

## Physics & Numerical Method
* **Photoelectric Emission:** Computes maximum initial electron kinetic energy ($K_{\max} = \frac{hc}{\lambda} - \Phi$) and emission velocity using Einstein's photoelectric equation for incident $450\text{ nm}$ photons on a sodium surface.
* **Kinematics Integration:** Solves the equations of motion ($\vec{F} = q\vec{E} = m_e\vec{a}$) via an **Euler-Cromer integration scheme** across discrete time steps ($\Delta t = 2.0 \times 10^{-11}\text{ s}$).
* **Visualization:** Renders continuous 2D particle trajectories overlaid on a spatial electric potential gradient map (`contourf`), demonstrating deceleration, turning points under retarding potentials, and plate collisions.

## Repository Structure
* `photoelectric_simulation.ipynb` — Main Jupyter Notebook containing the physics constants, ODE solver, and Matplotlib animation generator.
* `photoelectric_simulation.gif` — Exported animation loop showing electron deceleration and reversal under a $-6.0\text{ V}$ retarding potential.
* `requirements.txt` — Python dependencies required to run the simulation.

## Setup & Usage
1. **Clone the repository:**
   ```bash
   git clone [https://github.com/yourusername/photoelectric-effect-simulation.git](https://github.com/yourusername/photoelectric-effect-simulation.git)
   cd photoelectric-effect-simulation
