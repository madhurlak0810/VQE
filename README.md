# Nonlinear Variational Quantum Eigensolver (VQE) Project

## Introduction
The Variational Quantum Eigensolver (VQE) is a hybrid quantum-classical algorithm designed to approximate the ground state energy of a quantum system, with applications in quantum chemistry and physics. The optimization of VQE parameters presents a significant challenge due to its non-convex energy landscape, characterized by multiple local minima and barren plateaus. This project implements a **nonlinear VQE** variant, introducing nonlinearity through a parameterized ansatz with controlled gates and a nonlinear penalty in the objective function.

## Overview
This repository contains a Python implementation of a nonlinear VQE for a 10-qubit system, using Qiskit. Key features include:
- A synthetic 10-qubit Hamiltonian with \( ZZ \) and \( X \) terms.
- A nonlinear ansatz combining standard \( RY \) gates and controlled \( RY \) gates with \( \sin(\theta)^2 \) angles.
- A nonlinear objective function with a quadratic penalty term.
- Optimization via the Simultaneous Perturbation Stochastic Approximation (SPSA) algorithm.

The nonlinearity amplifies the non-convexity of the optimization landscape, making it a compelling case study for solving Optimization Problems: identifying a problem, formulating it mathematically, and solving it numerically.

## Prerequisites
- **Python**: 3.8 or higher
- **Qiskit**: Version 1.0 or later (includes `qiskit`, `qiskit-aer`, `qiskit-quantum-info`, `qiskit-primitives`)
- **NumPy**: For numerical operations

Install dependencies via pip:
```bash
pip install qiskit qiskit-aer numpy
