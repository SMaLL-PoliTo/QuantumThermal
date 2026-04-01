🚀 Case Study A2 — Ideal Quantum VQE Simulations (Quantum Matcha TEA)
----------------------------------------------------------------------------------------------------------------------------------------------------------------
This folder contains the simulation notebook and results for Case Study #2 from the associated publication.
These tests implement a Variational Quantum Eigensolver (VQE) using the **A2** ansatz, executed on the Quantum Matcha TEA framework under ideal (noise-free) conditions.

🧠 Ansatz — **A2** Configuration
----------------------------------------------------------------------------------------------------------------------------------------------------------------
| Property             | Description                                              |
| -------------------- | -------------------------------------------------------- |
| Ansatz               | $\mathrm{R_y}$ gates + CZ gates                          |
| Entanglement pattern | **Full entanglement** across all qubits                  |
| Layers               | **3.5 layers**                                           |
| Number of qubits     | **3-qubit**, **4-qubit**, and **5-qubit** configurations |
| Execution            | **Ideal simulation** (no noise)                          |
| Framework            | **Quantum Matcha TEA**                                   |
| Optimizer            | **BFGS** (default tolerance)                             |
| Readout              | Single evaluation per iteration ($\mathrm{N_R}=1$)       |
