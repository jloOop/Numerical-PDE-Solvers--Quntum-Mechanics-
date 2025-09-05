# Numerical-PDE-Solvers--Foundation-of-Quntum-Mechanics-
Here I present several Numerical PDE solvers due to the Schrodinger equation in 1 and 3 dimenssions with different potential and boundary conditions to answer some Fundamental and foundational questions in Quantum Mechanics.
Subsequent generated data is analyzed on CPU with python and some of the generated images and Gifs will be presented.
To write the scripts I used Python with focous mostly on Cuda and Cupy packages to work on GPU A100 and H200 on Cluster Helix.
The main mathematical approach to attack the numeric solver of Schrodinger equation as a PDE was Finite difference method such as Cracnk-Nicolson method, forward/backward/cenrtal finite method and related topics.



# Numerical PDE Solvers for Foundations of Quantum Mechanics

This repository contains Python-based numerical solvers for the Schrödinger equation in 1D to 3D in spatial and 1D in time, designed to explore fundamental questions in quantum mechanics, such as wave function evolution of finite size, tunneling, and spin-orbit effects under various potentials and boundary conditions.

## Key Features
1. **Solvers and Simulations**:  
   Implementations of finite difference methods (e.g., Crank-Nicolson, forward/backward/central differences) to solve the time-dependent Schrödinger equation. Supports 1D and 3D grids with different potential such as harmonic potentials, absorbing boundaries, and spinor extensions for spin-1/2 particles.

2. **Data Analysis and Visualization**:  
   Post-processing scripts analyze simulation data on CPU (using NumPy, SciPy, and Matplotlib). Outputs include probability distributions, Bohmian trajectories, and visualizations like contour plots, GIFs, and histograms of arrival times.

3. **Technology Stack**:  
   - Primary focus on GPU acceleration using CUDA via CuPy for high-performance simulations.  
   - Tested on NVIDIA A40, A100 and H200 GPUs on the Helix cluster, but includes CPU fallbacks.  
   - Core libraries: CuPy, NumPy, SciPy, Matplotlib. No external dependencies beyond Python 3.8+ and CUDA 11+ for GPU mode.

4. **Mathematical Approach**:  
   The solvers use mainly finite difference discretization for the PDE, with Crank-Nicolson for time-stepping to ensure stability and unitarity of big matrices with suitable boundary conditions include Dirichlet, Neumann, and Robin (absorbing) to answer some question regarding Bohmian mechanics and Bohmian trajectory of a particle in finite boxes.

## Getting Started

.....
