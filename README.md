# Quantum Computing for Thermal Science

This repository collects code and tutorial material related to quantum-computing applications in thermal science, with a particular focus on heat-conduction problems and linear-system formulations relevant to engineering.

The repository is connected to the broader document **"Notes on Quantum Computing for Thermal Science"** ([arXiv](https://arxiv.org/abs/2503.19109), [full document on GitHub](https://github.com/SMaLL-PoliTo/QuantumThermal/blob/main/notes.pdf)), which serves as a more complete compendium of the topics covered here. That document brings together and expands upon the material associated with the two paper-specific subfolders included in this repository.

![Quantum Computing for Thermal Science](https://github.com/SMaLL-PoliTo/QuantumThermal/blob/main/images/quantherm.png "Quantum Computing for Thermal Science")

## Repository structure

This repository is organized into two main subfolders:

- **`HHL/`**  
  Material related to the HHL tutorial paper, focused on the Harrow-Hassidim-Lloyd algorithm for linear systems and its application to a simple heat-conduction example. The corresponding notebooks are intended as pedagogical companions to the manuscript.

- **`VQE/`**  
  Material related to the VQE-based [paper](https://doi.org/10.1016/j.csite.2026.107813) published in *CSITE*, focused on variational quantum approaches for thermal-science problems.

## Scope

While the two subfolders correspond to two specific publications, readers interested in the broader context, derivations, and additional discussion are encouraged to refer to the full arXiv document:

**[Notes on Quantum Computing for Thermal Science](https://arxiv.org/abs/2503.19109)**

This document can be viewed as a unified reference that connects and extends the material associated with both the `HHL` and `VQE` parts of the repository.

## How to cite

If you found this material valuable, please consider citing the related arXiv document and papers:

- our *living* document exploring quantum computing in thermal science:
    > Asinari, P., Alghamdi, N., De Angelis, P., Barletta, G., Trezza, G., Provenzano, M., Piredda, M. M., Fasano, M. & Chiavazzo, E. (2025). Notes on Quantum Computing for Thermal Science. arXiv. DOI: [10.48550/arXiv.2503.19109](https://doi.org/10.48550/arXiv.2503.19109)
```bibtex
@article{asinari2025quantum,
  author  = {Asinari, P. and Alghamdi, N. and De Angelis, P. and Barletta, G. and Trezza, G. and Provenzano, M. and others and Chiavazzo, E.},
  title   = {Notes on Quantum Computing for Thermal Science},
  journal = {arXiv preprint arXiv:2503.19109},
  year    = {2025},
  doi     = {10.48550/arXiv.2503.19109}
}
```
- VQE-based [paper](https://doi.org/10.1016/j.csite.2026.107813) published in *CSITE*:
    > Asinari, P., Piredda, M. M., Barletta, G., De Angelis, P., Alghamdi, N., Trezza, G., Provenzano, M., Fasano, M. & Chiavazzo, E. (2026). Leveraging quantum computing for heat conduction analysis: A case study in thermal engineering. Case Studies in Thermal Engineering, 107813. DOI: [10.1016/j.csite.2026.107813](https://doi.org/10.1016/j.csite.2026.107813)
```bibtex
@article{asinari2025quantum,
  @article{asinari2026leveraging,
  title     = {Leveraging quantum computing for heat conduction analysis: A case study in thermal engineering},
  author    = {Asinari, Pietro and Piredda, Matteo Maria and Barletta, Giulio and De Angelis, Paolo and Alghamdi, Nada and Trezza, Giovanni and Provenzano, Marina and Fasano, Matteo and Chiavazzo, Eliodoro},
  journal   = {Case Studies in Thermal Engineering},
  pages     = {107813},
  year      = {2026},
  publisher = {Elsevier},
  doi       = {10.1016/j.csite.2026.107813}
}
```

## Authors

May 2025  
[Pietro Asinari](https://staff.polito.it/pietro.asinari/), [Nada Alghamdi](https://www.polito.it/en/staff?p=106642), [Paolo De Angelis](https://paolodeangelis.github.io/), [Giulio Barletta](https://giuliobarl.github.io/), [Giovanni Trezza](https://www.grenoble-inp.fr/fr/personnel/giovanni-trezza), [Marina Provenzano](https://www.polito.it/en/staff?p=043095), [Matteo Maria Piredda](https://www.polito.it/en/staff?p=067867), [Matteo Fasano](https://www.polito.it/en/staff?p=026208), [Eliodoro Chiavazzo](https://www.polito.it/en/staff?p=eliodoro.chiavazzo)