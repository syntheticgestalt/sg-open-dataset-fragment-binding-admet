# SyntheticGestalt Open Dataset: SPR-Based Fragment Binding and ADMET Properties

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Dataset](https://img.shields.io/badge/Dataset-Fragment%20Binding-blue.svg)](https://github.com/syntheticgestalt/spr-assay-fragment-screening-admet-data/tree/main/Data/Fragment_affinity)
[![Dataset](https://img.shields.io/badge/Dataset-ADMET%20Properties-green.svg)](https://github.com/syntheticgestalt/spr-assay-fragment-screening-admet-data/tree/main/Data/ADMET)

## Overview

This dataset contains fragment binding affinity data and ADMET (Absorption, Distribution, Metabolism, Excretion, Toxicity) property data obtained through the NEDO GENIAC project by SyntheticGestalt KK.

## 📊 Dataset Composition

### 1. Fragment Binding Affinity Data

Binding affinity data for 1,905 fragment compounds against four target proteins, measured using Surface Plasmon Resonance (SPR):

| Target Protein | Description | Hit Compounds | Reliable Kd Values |
|---|---|---|---|
| **BRD4** | Bromodomain-Containing Protein 4<br/>Epigenetic reader protein | 78 | 29 compounds with Kd < 1 mM |
| **NRP1** | Neuropilin-1<br/>Cell surface co-receptor | 192 | 66 compounds with Kd < 1 mM |
| **SKP1** | S-phase kinase-associated protein 1<br/>Component of SCF (SKP1–Cullin–F-box) complex | 98 | 6 compounds with Kd < 1 mM |
| **STING** | Stimulator of Interferon Genes<br/>Cytosolic adaptor protein central to the DNA-sensing pathway | 129 | 8 compounds with Kd < 1 mM |

### 2. ADMET Property Data

Pharmacokinetic and toxicity properties measured for 50 compounds:

| Property | Evaluation Method | Classification Criteria |
|---|---|---|
| **BBB Permeability** | Bidirectional permeability assay using MDR1-MDCKII cells | LogBB ≥ -1: Permeable (1) |
| **Microsomal Stability** | Metabolic stability assessment in human liver microsomes | t₁/₂ > 30 min: Stable (1) |
| **3T3 Phototoxicity** | Phototoxicity assay using NIH/3T3 mouse fibroblast cells | PIF < 2: Non-phototoxic (1) |

## 🔬 Experimental Methods

### Surface Plasmon Resonance (SPR)

- **Instrument**: Biacore 8K (Cytiva)
- **Chip**: Neutravidin (NA) sensor chip
- **Measurement Conditions**: 
  - Association phase: 30 seconds
  - Dissociation phase: 60-120 seconds
  - Compound concentrations: 50, 150, 500 µM (dose-response experiments)
- **Data Analysis**: Dissociation constants (Kd) determined based on the SPR response plotted against compound concentration

### ADMET Evaluation

#### BBB Permeability
- **Cell Line**: MDR1-MDCKII cells
- **Measurement**: Bidirectional permeability (Papp)
- **Conditions**: 37°C, 90-minute incubation
- **Detection**: LC-MS/MS

#### Microsomal Stability
- **Sample**: Pooled human liver microsomes
- **Conditions**: 37°C, up to 40 minutes
- **Time Points**: 0, 7, 15, 25, 40 minutes
- **Analysis**: HPLC-MS/MS

#### 3T3 Phototoxicity
- **Cell Line**: NIH/3T3 mouse fibroblast cells
- **UV-A Irradiation**: 5.5-6 J/cm²
- **Assessment**: Resazurin fluorescence assay
- **Determination**: Photo-Irritation Factor (PIF)

## 📁 Data Structure

```
sg-fragment-binding-admet-open-dataset/
├── README.md
└── Data/
    ├── ADMET/
    │   ├── 3T3_phototoxicity.csv
    │   ├── BBB_permeability.csv
    │   └── Microsomal_stability.csv
    └── Fragment_affinity/
        ├── BRD4.csv
        ├── NRP1.csv
        ├── SKP1.csv
        └── STING.csv
```

### Data Format

#### Fragment Binding Data
- `smiles`: Compound SMILES structure
- `binding_class`: Binary classification (1: Kd < 1 mM, 0: Kd ≥ 1 mM)

#### ADMET Property Data
- `compound_id`: Compound identifier
- `property_value`: Measured value
- `classification`: Binary classification (1: favorable, 0: unfavorable)
- `smiles`: Compound SMILES structure

## 📊 Statistical Summary

### Binding Affinity Distribution
- **BRD4**: Active compound rate 1.5% (29/1,905)
- **NRP1**: Active compound rate 3.5% (66/1,905)
- **SKP1**: Active compound rate 0.3% (6/1,905)
- **STING**: Active compound rate 0.4% (8/1,905)

### ADMET Property Distribution
- **BBB Permeability**: Permeable 98% (49/50)
- **Microsomal Stability**: Stable 70% (35/50)
- **3T3 Phototoxicity**: Non-toxic 90% (45/50)

## 📄 Citation

If you use this dataset in your research, please acknowledge:

> SyntheticGestalt Open Dataset: SPR-Based Fragment Binding and ADMET Properties. SyntheticGestalt Research Team. (2025). Available at: https://github.com/syntheticgestalt/sg-fragment-binding-admet-open-dataset

## 📜 License

This dataset is released under the MIT License. See [LICENSE](LICENSE) file for details.

## 🤝 Contributing

We welcome contributions for data quality improvements and new analytical approaches. Please use GitHub Issues or Pull Requests.

## 📞 Contact

- **Project**: NEDO GENIAC (Post-5G Information and Communication System Infrastructure Enhancement R&D Project)
- **Data Provider**: SyntheticGestalt KK.
- **Email**: info@syntheticgestalt.com
- **Website**: https://syntheticgestalt.com
- **GitHub**: https://github.com/syntheticgestalt/sg-fragment-binding-admet-open-dataset

---

> **Note**: This dataset is intended for research and educational purposes. For commercial use, please contact us separately.

> **Disclaimer**: We do not guarantee the accuracy or completeness of the experimental data. Users are responsible for the appropriate utilization of the data.
