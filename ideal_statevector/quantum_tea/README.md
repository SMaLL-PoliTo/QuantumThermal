🚀 Case Study A2 — Ideal Quantum VQE Simulations (Quantum Matcha TEA)
----------------------------------------------------------------------------------------------------------------------------------------------------------------
This folder contains the simulation code and results for Case Study #2 from the corresponding publication.
The experiments here implement a Variational Quantum Eigensolver (VQE) using the A2 ansatz, executed on the Quantum Matcha TEA framework under ideal (noise-free) conditions.

🧠 Ansatz — A2 Configuration
----------------------------------------------------------------------------------------------------------------------------------------------------------------
| Property             | Description                                     |
| -------------------- | ----------------------------------------------- |
| Ansatz               | `R_y` rotations + **CZ entangling gates**       |
| Entanglement pattern | **Full entanglement** across all qubits         |
| Layers               | **3.5 layers**                                  |
| Qubits tested        | **3-qubit, 4-qubit, and 5-qubit cases**         |
| Execution            | **Ideal simulation** (no noise)                 |
| Framework            | **Quantum Matcha TEA**                          |
| Optimizer            | **BFGS** (default tolerance)                    |
| Readout              | **Single evaluation per iteration** (`N_R = 1`) |
