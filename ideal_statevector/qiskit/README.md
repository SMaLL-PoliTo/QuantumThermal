🚀 Case Study A1 — Ideal Quantum VQE Simulations (Qiskit)
--------------------------------------------------------------------------------------------------------------------------------------------
This folder contains the simulation notebook and results for Case Study #1 from the associated publication.
These tests implement a Variational Quantum Eigensolver (VQE) using the **A1** ansatz presented in the paper, evaluated under ideal (noise-free) conditions with Qiskit.

🧠 Ansatz — **A1** Configuration
--------------------------------------------------------------------------------------------------------------------------------------------
| Property             | Description                                   |
| -------------------- | --------------------------------------------- |
| Ansatz               | `$R_y$` and `$R_z$` gates + `CX` gates        |
| Entanglement pattern | **Linear entanglement** across qubits         |
| Layers               | **3.5 layers**                                |
| Number of qubits     | **3-qubit** and **4-qubit** configurations    |
| Execution            | **Ideal simulator** (no noise, no shots)      |
| Framework            | **Qiskit**                                    |
| Optimizer            | **COBYLA**                                    |
| COBYLA tolerance     | `1e-3` (3 qubits), `1e-6` (4 qubits)          |
| Readout              | Single evaluation per iteration (`$N_R$ = 1`) |
