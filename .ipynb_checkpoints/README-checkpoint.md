# Fault-Tolerant Quantum Compilation (FTQC) Pipeline
## Overview
This project demonstrates a full-stack quantum compilation pipeline, focusing on transforming continuous quantum algorithms (like Trotterized chemistry benchmarks) into fault-tolerant executable formats. 
## Key Features
* **Clifford+T Synthesis:** Utilized the Solovay-Kitaev algorithm to discretize arbitrary rotations.
* **T-Count Optimization:** Applied ZX-calculus graph theory via `PyZX` to drastically reduce logical T-gate overhead.
* **Hardware Routing:** Mapped logical circuits onto constrained physical topologies using Qiskit pass managers.
* **Resource Estimation:** Extracted and visualized depth overhead and gate metrics across the pipeline.
## Tech Stack
* Python 3.10
* Qiskit
* PyZX
* Matplotlib
