🚀 Case Study A3p — Qrisp VQE With COBYQA (Precision Comparison)
---------------------------------------------------------------------------------------------------------------------------------
This folder contains the simulation notebook and results for Case Study #5 and #6 from the publication.
Both tests evaluate a Variational Quantum Eigensolver (VQE) implemented in Qrisp, using:

- **A3p** ansatz

- COBYQA optimizer

- 3 qubits

- 4 ansatz layers

- Full entanglement topology

The goal is to analyze numerical precision effects in quantum-classical optimization with a noise-free statevector backend.

🧠 Ansatz — **A3p** Configuration
---------------------------------------------------------------------------------------------------------------------------------
| Property             | Description                             |
| -------------------- | --------------------------------------- |
| Ansatz               | $\mathrm{R_y}$ gates + CX gates         |
| Entanglement pattern | **Full entanglement** across all qubits |
| Layers               | 4                                       |
| Number of qubits     | **3 qubits** configuration              |
| Execution            | **Shot-based simulation**               |
| Framework            | **Qrisp** statevector simulator         |
| Optimizer            | COBYQA                                  |
| Hamiltonian          | $\mathrm{H_2}$ molecule (minimal basis) |
| Readout              | $\mathrm{N_R}=30$ independent restarts  |

🔍 Case #5 vs Case #6 — Key Difference
---------------------------------------------------------------------------------------------------------------------------------
| Case        | Framework | Precision Setting                                            | Notes                                       |
| ----------- | --------- | ------------------------------------------------------------ | ------------------------------------------- |
| **Case #5** | Qrisp     | Default COBYQA precision                                     | Baseline high-precision configuration       |
| **Case #6** | Qrisp     | **Reduced numerical precision** (looser optimizer tolerance) | Tests stability under precision constraints |
