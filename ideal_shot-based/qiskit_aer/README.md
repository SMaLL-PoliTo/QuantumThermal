🚀 Case Study A3 — Shot-Based VQE Simulations (Qiskit Aer)
---------------------------------------------------------------------------------------------------------------------------------------------------
This folder contains the simulation notebook and results for Case Study #3 and #4 from the associated publication.
Both tests implement a Variational Quantum Eigensolver (VQE) using the **A3** ansatz under realistic shot-based sampling on the Qiskit Aer simulator.

These experiments evaluate the effect of sampling noise by varying the number of measurement shots.

🧠 Ansatz — **A3** Configuration
---------------------------------------------------------------------------------------------------------------------------------------------------
| Property             | Description                            |
| -------------------- | -------------------------------------- |
| Ansatz               | `R<sub>y</sub>` gates + `CX` gates     |
| Entanglement pattern | **Full entanglement** across qubits    |
| Layers               | **4 layers**                           |
| Number of qubits     | **3 qubits** configuration             |
| Execution            | **Shot-based simulation**              |
| Framework            | **Qiskit Aer**                         |
| Optimizer            | **COBYQA**                             |
| Readout              | `N<sub>R</sub> = 30`                   |

📌 Difference Between Case #3 and #4
---------------------------------------------------------------------------------------------------------------------------------------------------
| Case        | Shots           | Notes                                   |
| ----------- | --------------- | --------------------------------------- |
| **Case #3** | **1,024 shots** | Baseline noisy simulation               |
| **Case #4** | **4,096 shots** | Higher accuracy, reduced sampling noise |

Higher shots → Lower noise → Better convergence (but slower runtime)
