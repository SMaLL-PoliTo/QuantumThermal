# HHL Follow-Up Tutorial Notebooks (Qiskit)

This repository contains the two Jupyter notebooks that accompany the follow-up tutorial paper on the Harrow-Hassidim-Lloyd (HHL) algorithm.

The material is designed to complement the manuscript by providing a practical, notebook-based walkthrough in **Qiskit** of:

1. **real data loading / amplitude encoding** for a small input register, and
2. a full **ideal HHL statevector simulation** for the heat-conduction example discussed in the paper.

The notebooks are intended for **pedagogical use**. They prioritize clarity and consistency with the manuscript over computational efficiency or hardware-oriented execution.

## Repository contents

This repository contains only the following two notebooks:

- `real-data-loader_qiskit_run3q.ipynb`  
  Tutorial notebook showing how real-valued data can be loaded into a **3-qubit input register** using a divide-and-conquer amplitude-encoding strategy in Qiskit.

- `HHL_qiskit_run3q_clock5q_ancilla1q.ipynb`  
  Main HHL tutorial notebook implementing the heat-equation example with **3 input qubits**, **5 clock qubits**, and **1 ancilla qubit**, using ideal statevector simulations.

## What the notebooks cover

### 1. Real data loader notebook
This notebook illustrates how a real-valued vector can be encoded into a quantum state using controlled `RY` rotations. It is meant as supporting material for the appendix on real data loading/encoding.

### 2. HHL tutorial notebook
This notebook follows the structure of the manuscript and walks through the main stages of the HHL algorithm:

- problem definition and normalization,
- spectral analysis of the test matrix,
- quantum phase estimation (QPE),
- eigenvalue inversion through controlled rotations,
- inverse QPE and uncomputation,
- post-selection,
- reconstruction of the solution and comparison with the classical reference.

## Scope and limitations

- The notebooks use **ideal simulations**, mainly through statevector analysis.
- They are meant to explain the internal logic of HHL, not to provide an optimized or hardware-ready implementation.
- The example is intentionally small so that intermediate states, eigenvalue mappings, and probability distributions can be inspected clearly.

## Suggested environment

A standard Python environment with Jupyter and Qiskit is sufficient. In practice, you will typically need:

- Python 3
- Jupyter Notebook or JupyterLab
- Qiskit
- NumPy
- Matplotlib
- SciPy

Depending on your local setup, some additional packages used by Qiskit visualizations may also be helpful.

## How to use the repository

A reasonable reading order is:

1. start from `real-data-loader_qiskit_run3q.ipynb`,
2. then move to `HHL_qiskit_run3q_clock5q_ancilla1q.ipynb`.

This order mirrors the pedagogical progression of the manuscript: first state preparation, then the full HHL workflow.

## Relation to the manuscript

These notebooks accompany the follow-up HHL tutorial paper and are meant to support the practical understanding of the derivations presented there. In particular:

- the real-data-loader notebook supports the appendix on **real data loading/encoding**,
- the HHL notebook supports the main worked example based on the **1D heat-conduction problem**.

## Notes

The notebooks were prepared for tutorial purposes. For this reason, some cells include extra intermediate outputs, explicit checks, and comparisons between theoretical models and simulated results.

## How to cite

If you found this valuable, please consider citing the related paper.

Additionally, please refer to (and consider citing):

- the tutorial by Zaman et al.:
    > Zaman, A., Morrell, H. J., & Wong, H. Y. (2023). A step-by-step HHL algorithm walkthrough to enhance understanding of critical quantum computing concepts. IEEE Access, 11, 77117-77131. DOI: [10.1109/ACCESS.2023.3297658](https://doi.org/10.1109/ACCESS.2023.3297658)
```bibtex
@article{zaman2023hhl,
  author  = {Zaman, A. and Morrell, H. J. and Wong, H. Y.},
  title   = {A step-by-step HHL algorithm walkthrough to enhance understanding of critical quantum computing concepts},
  journal = {IEEE Access},
  volume  = {11},
  pages   = {77117--77131},
  year    = {2023},
  doi     = {10.1109/ACCESS.2023.3297658}
}
```
- our *living* document exploring quantum computing in thermal science:
    > Asinari, P., Alghamdi, N., De Angelis, P., Barletta, G., Trezza, G., Provenzano, M., ... & Chiavazzo, E. (2025). Notes on Quantum Computing for Thermal Science. arXiv preprint arXiv:2503.19109. DOI: [10.48550/arXiv.2503.19109](https://doi.org/10.48550/arXiv.2503.19109)
```bibtex
@article{asinari2025quantum,
  author  = {Asinari, P. and Alghamdi, N. and De Angelis, P. and Barletta, G. and Trezza, G. and Provenzano, M. and others and Chiavazzo, E.},
  title   = {Notes on Quantum Computing for Thermal Science},
  journal = {arXiv preprint arXiv:2503.19109},
  year    = {2025},
  doi     = {10.48550/arXiv.2503.19109}
}
```
