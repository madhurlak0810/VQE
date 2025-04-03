# Nonlinear Variational Quantum Eigensolver (VQE) Project

## Introduction
The Variational Quantum Eigensolver (VQE) is a hybrid quantum-classical algorithm designed to approximate the ground state energy of a quantum system, with applications in quantum chemistry and physics. The optimization of VQE parameters presents a significant challenge due to its non-convex energy landscape, characterized by multiple local minima and barren plateaus. This project implements a **nonlinear VQE** variant, introducing nonlinearity through a parameterized ansatz with controlled gates and a nonlinear penalty in the objective function.

## Overview
# Nonlinear Variational Quantum Eigensolver (VQE) for a 10-Qubit System

This repository contains a **Python implementation** of a **nonlinear Variational Quantum Eigensolver (VQE)** for a **10-qubit system**, using **Qiskit**.  

## Key Features  

- **Synthetic 10-Qubit Hamiltonian**  
  - Composed of \( ZZ \) and \( X \) interaction terms.  

- **Nonlinear Ansatz**  
  - Utilizes standard **\( RY \) gates**.  
  - Incorporates **controlled \( RY \) gates** with angles proportional to \( \sin(\theta)^2 \).  

- **Nonlinear Objective Function**  
  - Includes a **quadratic penalty term** to introduce additional complexity.  

- **Optimization via SPSA Algorithm**  
  - Employs the **Simultaneous Perturbation Stochastic Approximation (SPSA)** method for parameter optimization.  

## Why Nonlinearity?  

The introduced nonlinearity **intensifies the non-convexity** of the optimization landscape, making this approach a compelling **case study in solving complex optimization problems**. It highlights the full pipeline of:  

1. **Identifying a Problem**  
2. **Formulating it Mathematically**  
3. **Solving it Numerically**  

This implementation provides a valuable testbed for exploring **quantum optimization techniques** and their practical implications.  

---


## Prerequisites
- **Python**: 3.8 or higher
- **Qiskit**: Version 1.0 or later (includes `qiskit`, `qiskit-aer`, `qiskit-quantum-info`, `qiskit-primitives`)
- **NumPy**: For numerical operations

Install dependencies via pip:
```bash
pip install qiskit qiskit-aer numpy
