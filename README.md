# SU(5) Phase-Field Cosmology & Topological Matter Simulations

This repository contains the high-resolution, GPU-accelerated PyTorch tensor simulations supporting the phenomenological framework of spacetime as an oscillatory $SU(5)$ phase field.

### Author
**Simeon Ivaylov Petrov** Team Leader & Web Developer | BSc Computer Science | Sofia, Bulgaria

### Overview
These notebooks utilize PyTorch's `float64` Autograd engine to compute 4th-order spatial finite differences across massive ($128^3$) 3D grids. By evaluating the non-linear sigma model alongside Faddeev-Skyrme geometric stabilization and explicit chiral symmetry breaking ($m_\pi = 0.15$), these simulations prove that Derrick's Theorem can be defeated on a discretized lattice, halting vacuum collapse.

### Files
1. **`1_B1_Particle_Crystallization.ipynb`**: Demonstrates the stabilization of a $B=1$ topological seed into a massive fundamental fermion ($E_{rest} \approx 7.24$).
2. **`2_DT_Nuclear_Fusion.ipynb`**: Demonstrates the stereographic merging of $B=2$ (Deuterium) and $B=3$ (Tritium) seeds. The simulation naturally captures the strong force energy drop and the geometric decay of the unstable $B=5$ state into a $B=4$ Alpha particle and a $B=1$ fast neutron.

### Usage
These notebooks are designed to be run directly in Google Colab using a T4 GPU (or higher) with at least 16GB of VRAM.
