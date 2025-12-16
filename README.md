# Deep Learning Final Project

This repository contains code and tools for solving the steady-state 2D convection–diffusion equation with Physics-Informed Neural Networks (PINNs). The work introduces and evaluates modified PINN architectures designed to improve accuracy and convergence relative to a standard fully connected PyTorch PINN baseline.
## Overview
This repository presents a reproducible study of architectural choices for PINNs applied to a steady-state convection–diffusion problem. A high-resolution finite-difference solver is used to generate reference solutions on a unit square domain, against which multiple PINN architectures are trained and evaluated under identical PDE constraints and boundary conditions. Model predictions are compared to the numerical reference to assess improvements in accuracy and convergence behavior relative to a baseline PyTorch PINN.

## Architectures and Results
**`index.html`** presents the studied architectures along with a summary of quantitative and qualitative results. This includes comparisons between the following:
- A standard fully connected PINN
- Split architectures with separate advection and diffusion branches
- Gated and additive coupling strategies
- Feature-mixing approaches

## Repository Contents
- Finite-difference solver for reference data generation  
- `Github_PINNs.ipynb` containing PINN architectures
- `index.html` summarizing architectures, experiments, and results
