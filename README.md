# TCM-MS2Link: A Unified Dataset Integrating TCM Herb–Compound Knowledge and MS/MS Spectral Data

<p align="center">
  <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="License"></a>
  <a href="https://github.com/NIM-NMDC/TCM-MS2Link"><img src="https://img.shields.io/badge/Dataset-TCM--MS2Link-blue.svg" alt="Dataset"></a>
  <a href="https://pytorch.org/"><img src="https://img.shields.io/badge/PyTorch-EE4C2C.svg?logo=pytorch&logoColor=white" alt="PyTorch"></a>
</p>

<p align="center">
  <img src="fig/TCM-MS2Link.png" alt="RFDD Dataset Cover" width="100%"/>
</p>

**TCM-MS2Link** adopts a dual-layer “knowledge–data” architecture: the first layer, **TCM-MolLink**, comprises curated herb–compound association data, constructed through the integration of multiple heterogeneous databases and rigorous consistency filtering to establish high-confidence relationships between TCM herbs and their chemical constituents; the second layer, **MS2-MLReady**, is a benchmark dataset for mass spectrometry–based machine learning, which, after systematic data cleaning, standardized preprocessing, and well-designed data partitioning, can directly support the training and evaluation of artificial intelligence models.

> **📢 Notice**: Both the **complete dataset** and **source code** will be fully released upon the official acceptance of our paper.

---

## 📊 Dataset Info

|   Dataset    | Format | Records |                  Description                   |
| :----------: | :----: | :-----: | :--------------------------------------------: |
| TCM-MolLink  |  CSV   | 12,625  | High-confidence herb–compound association data |
| TCM-MS2Clean |  TSV   | 325,530 |          Curated MS/MS spectral data           |
| MS2-MLReady  |  TSV   | 284,729 |        Subset of [M+H]+ adduct spectra         |

The fully curated MS/MS dataset, **TCM-MS2Clean**, is provided as a supplementary resource. MS2-MLReady is derived from TCM-MS2Clean by retaining only spectra with the adduct type **[M+H]+**.

---

## 🔍  Discussion

These figures demonstrate that compounds in the MS2-MLReady dataset predominantly fall within the drug-like chemical space.

<img src="fig/Figure1.png" style="zoom: 35%;" />

<img src="fig/Figure2.png" style="zoom:25%;" />


*The distributions of key physicochemical properties (MW, LogP, TPSA, HBD, and HBA), along with the PCA visualization of chemical space, indicate that the majority of compounds in the MS2-MLReady dataset fall within the typical drug-like region. This observation is broadly consistent with the criteria of Lipinski's Rule of Five, suggesting that the dataset primarily represents chemically relevant space for small-molecule drug discovery.*

---

## 📜 Citation

If you find TCM-MS2Link useful for your research, please cite:

```bibtex
@article{TCM-MS2Link2026,
  title   = {TCM-MS2Link: A Unified AI-Ready Dataset Integrating TCM Herb–Compound Knowledge and MS/MS Spectral Data},
  author  = {Qianjin Li},
}
