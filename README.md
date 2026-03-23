# SU(2) Subsector Simulations  
for the SU(5) Phase-Field Phenomenological Prototype

This repository contains the GPU-accelerated PyTorch notebooks that support the phenomenological framework presented in the paper  
**“Spacetime as an Oscillatory Phase Field: A Phenomenological SU(5) Prototype…”** (TOE (11), dated 23 March 2026).

All simulations are performed exclusively in the **reduced SU(2) ≃ O(4) topological subsector**. They are not full SU(5) dynamics and should be interpreted as numerical evidence for mechanism viability (stabilization, binding, seed formation, and qualitative nuclear analogues), not as proofs of physical reality.

### Author
**Simeon Ivaylov Petrov**  
BSc Computer Science, Sofia, Bulgaria

### Notebooks

0. **`0_Kibble-Zurek_Engine.ipynb`**  
   Simulates the 3D post-inflationary quench on a 128³ lattice. Demonstrates domain-wall formation, coarsening, and the spontaneous emergence of localized regions carrying nontrivial winding (supporting the Kibble–Zurek-type seed-formation scenario in the paper).

1. **`1_B1_Particle_Crystallization.ipynb`**  
   Evolves a single B ≈ 1 hedgehog seed under constrained gradient flow. Shows stabilization of a localized topological defect at a nonzero rest-mass plateau while preserving winding number (illustrating how the fourth-order Skyrme term can overcome Derrick’s theorem in the lattice discretization).

2. **`2_DT_Nuclear_Fusion.ipynb`**  
   Merges B = 2 and B = 3 configurations via stereographic product ansatz. Exhibits energy relaxation and spontaneous reorganization of the unstable intermediate into a more stable remnant plus emitted fragment (qualitative analogue of D–T fusion).

3. **`3_Heavy_Nuclei_Crystallization.ipynb`**  
   Explores higher-charge states. By tuning the effective pion mass and Skyrme coefficient, a B = 7 configuration can be stabilized for extended relaxation time, indicating a stability window for heavier polyhedral configurations.

4. **`4_Matter_Antimatter_Annihilation.ipynb`**  
   Collides a B = 1 seed with a B = −1 seed. Demonstrates topological charge cancellation to numerical precision and conversion of rest energy into high-frequency field oscillations (consistency check for matter–antimatter behaviour in the reduced model).

### Usage Instructions
- Run directly in **Google Colab** (T4 GPU or better recommended).  
- Use `torch.float64` precision (already set in the notebooks).  
- **Important**: Due to high VRAM usage on 128³ grids, restart the Colab session between notebooks to clear the GPU cache.

### Relation to the Paper
These notebooks provide the numerical backbone for Sections IV, VII–IX of TOE (11). All results are described qualitatively in the paper; the notebooks allow anyone to reproduce and extend the simulations.

The framework remains phenomenological. Full SU(5) dynamics, first-principles derivation of the macroscopic potential, and a realistic particle spectrum are left for future work (see Section X of the paper for a detailed discussion of scope and limitations).

**Paper (latest version):**  
[TOE (11) PDF](https://github.com/sipy/su5-phase-field/blob/main/TOE_(11).pdf) *(or the version linked in the arXiv preprint if uploaded)*

---

Last updated: 23 March 2026
