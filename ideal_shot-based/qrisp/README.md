🚀 Case Study A3p — Qrisp VQE With COBYQA (Precision Comparison)
---------------------------------------------------------------------------------------------------------------------------------
This folder contains the code for Case Study #5 and #6 from the publication.
Both cases evaluate a Variational Quantum Eigensolver (VQE) implemented in Qrisp, using:

- A3p ansatz

- COBYQA optimizer

- 3 qubits

- 4 ansatz layers

- Full entanglement topology

The goal is to analyze numerical precision effects in quantum-classical optimization with a noise-free statevector backend.

🧠 Ansatz — A3 Configuration
---------------------------------------------------------------------------------------------------------------------------------
| Property         | Description                                          |
| ---------------- | ---------------------------------------------------- |
| Ansatz           | `R_y` parameterized gates + full entangling CX gates |
| Layers           | 4                                                    |
| Connectivity     | Fully entangled                                      |
| Backend          | Qrisp statevector simulator                          |
| Optimizer        | COBYQA                                               |
| Hamiltonian      | H₂ molecule (minimal basis)                          |
| Convergence runs | `N_R = 30` independent restarts                      |

🔍 Case #5 vs Case #6 — Key Difference
---------------------------------------------------------------------------------------------------------------------------------
| Case        | Framework | Precision Setting                                            | Notes                                       |
| ----------- | --------- | ------------------------------------------------------------ | ------------------------------------------- |
| **Case #5** | Qrisp     | Default COBYQA precision                                     | Baseline high-precision configuration       |
| **Case #6** | Qrisp     | **Reduced numerical precision** (looser optimizer tolerance) | Tests stability under precision constraints |

