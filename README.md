# SnSe Photonic Memristors

**Two-Dimensional SnSe Photonic Memristors: A Graphene-Templated Ionic Crystal Architecture for Post-Von Neumann Computing**

Gabriel Reiser — Independent Researcher

---
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.19836411.svg)](https://doi.org/10.5281/zenodo.19836411)
## Overview

This repository contains the paper and supporting simulation notebooks for a theoretical architecture proposal for photonic memristors based on two-dimensional tin(II) selenide (SnSe) crystals fabricated on graphene substrates.

The core argument: the von Neumann bottleneck is a consequence of using electrons as the information medium. SnSe — a non-toxic, room-temperature ferroelectric van der Waals crystal — exhibits the intrinsic properties required for a genuinely photonic memory element. The photonic state is simultaneously the storage state and the computational state.

**Key claims (with explicit assumptions stated throughout):**
- Practical analog storage of ~4.3 bits/cell at conservative noise derate (vs 3 bits TLC NAND)
- Single layer areal density: ~8.22 Gbits/cm²
- Stack density scales as N complementary layer pairs (N experimentally undetermined)
- Antimony (Sb) identified as preferred dopant over bismuth (Bi) on manufacturing grounds
- Sb-Se chemistry validated at commercial scale in photovoltaic literature (Sb2Se3, Sb2(S,Se)3)

---

## Repository Contents

```
paper/
    photonic_memristor.docx    — Full paper draft
    photonic_memristor.pdf    — Full paper draft

notebooks/
    snse_photonic_memristor_simulations.ipynb  — Supporting simulations
```

---

## Simulations

The notebook contains three reproducible simulations:

1. **Optical Phase** — Bit depth derivation from measured SnSe birefringence (delta_n = 0.4, Guo et al. 2023)
2. **LGD Ferroelectric Switching** — Cone of operationality for switching voltage and retention, validated against Wang et al. 2024
3. **Sb vs Bi Dopant Comparison** — Manufacturing feasibility analysis with five testable predictions

Every parameter is labeled MEASURED, ESTIMATED, or ASSUMED. Modify any value and rerun to test sensitivity.

### Run the notebook

```bash
pip install numpy matplotlib jupyter
jupyter notebook notebooks/snse_photonic_memristor_simulations.ipynb
```

---

## Status

This is a theoretical architecture proposal, not a demonstrated experimental result. The paper makes specific, falsifiable predictions that define an experimental agenda. The simulations are supporting calculations, not proof.

Pending: arXiv submission (endorsement in physics.optics sought)

---

## Citation

If you use this work, please cite:

> Reiser, G. (2026). Two-Dimensional SnSe Photonic Memristors: A Graphene-Templated Ionic Crystal Architecture for Post-Von Neumann Computing. Independent Research. GitHub: github.com/gabereiser/snse-photonic-memristor


---

## License

This work is licensed under Creative Commons Attribution 4.0 International (CC BY 4.0).
You are free to share and adapt with attribution.
