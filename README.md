# Cross-Scale Mapping of Spatial Transcriptomics Data via Unbiased Cell Typing and Differential Gene Signature Overlap for Transferable Biological Interpretation

This repository contains code supporting the manuscript:

**“Transferable biological interpretation through cross-scale and cross-platform mapping of spatial transcriptomic datasets”**,  
submitted to ISMB 2026 proceedings.

---

## Overview

The analysis consists of four main components:

- **Unbiased Recursive Cell Typing (RCT)**
- **Mapping of unbiased cell types via differential gene signatures**
- **Spatial microdomain discovery**
- **Mapping of spatial interactions via unbiased cell types**

---

## Repository Structure

This repository contains the following directories:

- `Data/` – input data tables used in the analysis  
- `Figures/` – generated figures corresponding to manuscript results  
- `Modules/` – auxiliary modules  
- `Output/` – intermediate and final outputs  
- `src/` – core source code  

---

## Main Analysis Code

The primary analysis is executed via:

- `Banovich_IPF_analysis_clean.ipynb` – end-to-end analysis notebook  
- `recursive_celltyping.py` – unbiased recursive cell typing implementation  
- `Microdomain_discovery.py` – spatial microdomain inference  

---

## Dependencies

Key dependencies include (additional packages are required; see scripts and notebook for details):

- `CellGraph`
- `DeterministicPhenoGraph`
- `pvclust`

---

## Input Data

Input data expected under the `Data/` directory:

- `IPF_patient_ids.csv`
- `banovich_exprDF_annotmapped.parquet`
- `thomas_geneDF.parquet`
- `thomas_annotDF.parquet`

Data files are derived from publicly available datasets described in the manuscript.  
This repository does **not** redistribute raw experimental data beyond processed tables used for analysis.

---

## Figure Generation

All manuscript figures can be reproduced by running:

```bash
Banovich_IPF_analysis_clean.ipynb
