# Data: Generative Pipeline for Discovering Solid-State Battery Materials with Universal Atomistic Potentials

[![ICML 2026 AI4Science Workshop](https://img.shields.io/badge/ICML2026-AI4Science%20Workshop-blue)](https://openreview.net/forum?id=xFI6K4ZQDp)

## Overview

This repository contains data accompanying our contribution to the **ICML 2026 AI4Science Workshop**:

> **Generative Pipeline for Discovering Solid-State Battery Materials with Universal Atomistic Potentials**
> [OpenReview](https://openreview.net/forum?id=xFI6K4ZQDp)

We introduce a computational pipeline for discovering protective coating materials for Li-ion solid-state batteries. Starting from 527,365 element-constrained generated ternary crystal structures, a multi-stage screening workflow — combining universal machine learning interatomic potentials (uMLIPs), thermodynamic stability analysis, electrochemical compatibility checks, and Li-ion transport descriptors — narrows the candidate pool down to **29 structures** warranting further ab initio evaluation.

## Repository Structure

```
data/
├── candidates_AC.csv   # Anode coating candidates (extended Table 2)
└── candidates_CC.csv   # Cathode coating candidates (extended Table 3)
```

## Data Description

Both CSV files extend the corresponding tables in the paper with an additional column containing the crystal structure encoded in **CIF** format.

## Citation

If you use this data, please cite our workshop contribution:

```bibtex
@inproceedings{
  dembitskiy2026generative,
  title={Generative Pipeline for Discovering Solid-State Battery Materials with Universal Atomistic Potentials},
  author={Artem Dembitskiy and Shuya Yamazaki and Artem Maevskiy and Nikita Kazeev and Roman A. Eremin and Semen Budennyy and Kedar Hippalgaonkar and Antonio Helio Castro Neto and Andrey E Ustyuzhanin},
  booktitle={ICML 2026 AI for Science Workshop},
  year={2026},
  url={https://openreview.net/forum?id=xFI6K4ZQDp}
}
```

## Notes

The 29 candidates reported here are subject to further validation. We recommend density functional theory calculations of dynamical stability, interfacial properties, and charge-transfer mechanisms prior to any experimental synthesis. Please refer to the paper for a full discussion of the pipeline's limitations and directions for future work.

## License

The data in this repository is released under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
