🚀 Case Study A1 — Ideal Quantum VQE Simulations (Qiskit)
--------------------------------------------------------------------------------------------------------------------------------------------
This folder contains the simulation scripts corresponding to Case Study #1 in the associated publication.
These tests implement a Variational Quantum Eigensolver (VQE) using the A1 ansatz, evaluated under ideal (noise-free) conditions with Qiskit.

🧠 Ansatz — A1 Configuration
--------------------------------------------------------------------------------------------------------------------------------------------
| Property          | Description                                        |
| ----------------- | -------------------------------------------------- |
| Ansatz            | `R_y` and `R_z` gates + `CX` (linear entanglement) |
| Layers            | **3.5 layers**                                     |
| Number of qubits  | **3-qubit** and **4-qubit** configurations         |
| Execution backend | **Ideal Qiskit simulator** (no noise, no shots)    |
| Optimizer         | **COBYLA**                                         |
| COBYLA tolerance  | `1e-3` (3 qubits), `1e-6` (4 qubits)               |
| Readout           | Single evaluation per cost evaluation (`N_R = 1`)  |
