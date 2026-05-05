[README_sds_risk_pipeline.md](https://github.com/user-attachments/files/27417294/README_sds_risk_pipeline.md)

# SDS Risk Analysis Pipeline

## Overview

This repository contains the analytical pipeline, figure generation code, and supplemental table workflows associated with the manuscript:

> **Beyond Symptoms: Discrete Decision Windows Govern SDHI Seed Treatment Efficacy in Soybean Sudden Death Syndrome**

The project integrates molecular diagnostics, mixed-effects modeling, multivariate analyses, and economic risk stratification to investigate relationships among *Fusarium virguliforme*, soybean cyst nematode (SCN), disease development, and soybean yield across multistate field experiments conducted from 2020–2024.

---

## Repository Structure

```text
project/
├── data/
├── figures/
├── output/
├── scripts/
├── sds_risk_ms_pipeline_clean_annotated_bells_whistles.Rmd
├── README.md
└── .gitignore
```

### Directory Descriptions

| Folder | Description |
|---|---|
| `data/` | Raw and processed datasets used for analysis |
| `figures/` | Exported manuscript-quality figures |
| `output/` | Intermediate model outputs and tables |
| `scripts/` | Optional helper scripts and utilities |

---

## Main Pipeline

The primary workflow is contained in:

```text
sds_risk_ms_pipeline_clean_annotated_bells_whistles.Rmd
```

This annotated RMarkdown file includes:

- Data import and cleaning
- Feature engineering
- Linear mixed-effects modeling
- Correlation and network analyses
- Principal component analysis (PCA)
- Response surface analyses
- Decision-window / ROI modeling
- Figure generation and export
- Supplemental table generation
- Mapping workflows for manuscript Figure 1

---

## Study Scope

Field experiments were conducted from 2020–2024 across:

- 11 U.S. states
- Ontario, Canada
- 102 site-years

The dataset integrates:

- *Fusarium virguliforme* qPCR abundance
- SCN population density
- Root and foliar disease assessments
- Soil variables
- Yield outcomes
- Seed treatment responses

---

## Required R Packages

Core packages used in the workflow include:

```r
tidyverse
lme4
lmerTest
performance
rstatix
FactoMineR
factoextra
patchwork
maps
```

Additional packages may be required for specialized visualization or exploratory analyses.

---

## Running the Pipeline

1. Clone the repository
2. Place required datasets into the `data/` directory
3. Update file paths if necessary
4. Open the `.Rmd` file in RStudio
5. Run sequentially or knit the document

---

## Manuscript Outputs

The pipeline generates:

- Manuscript figures
- Supplemental tables
- Mixed-model outputs
- PCA visualizations
- ROI / decision-window analyses
- Geographic site-year maps

Annotated comments throughout the workflow identify which code blocks correspond to manuscript figures, tables, and supplemental outputs.

---

## Reproducibility Notes

- All analyses were conducted in R
- Figure export blocks are included throughout the workflow
- File paths may require modification for local environments
- The repository is structured to facilitate reproducibility and manuscript revision

---

## Citation

If using or adapting this workflow, please cite the associated manuscript once published.

---

## Contact

Ryan Hamilton  
Department of Plant, Soil and Microbial Sciences  
Michigan State University
