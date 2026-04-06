[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.19444965.svg)](https://doi.org/10.5281/zenodo.19444965)
# alpha-synuclein-evolution
Intra-Individual α-Synuclein Strain Maturation Underlies the Transition to Parkinson's Dementia 
## Overview
This pipeline analyzes peptide biomarkers across three independent datasets:
- Cross-sectional cohort (HC, NC, MCI, PDD)
- Longitudinal patient 149 (V1–V9)
- Mouse model (NCE, NCL, DE)

## Requirements
Install required packages:
pip install pandas numpy matplotlib seaborn scipy openpyxl

## Input Data
| File | Description |
|------|-------------|
| `For data analysis total.xlsx` | Raw peptide intensity data (all cohorts) |

## How to Run
Open `asyn_fingerprint_final.ipynb` in Jupyter Notebook or Google Colab and run all cells sequentially.

## Output Files
| File | Description |
|------|-------------|
| `PD_Proteomics_01_Preprocessed_Data.xlsx` | Normalized data (Log2, Z-score) |
| `PD_Proteomics_02_Heatmaps.pdf` | Heatmap visualizations |
| `PD_Proteomics_03_Pattern_Analysis.pdf` | Monotonic pattern analysis |
| `PD_Proteomics_03_Pattern_Results.xlsx` | Pattern classification results |
| `PD_Proteomics_04_Trajectory_Analysis.pdf` | Anchored trajectory analysis |
| `PD_Proteomics_04_Trajectory_Results.xlsx` | NCL projection results |

## Analysis Steps
1. **Preprocessing** – ENOLASE normalization → row median → Log2 → Z-score
2. **Heatmap Visualization** – individual samples and group averages
3. **Pattern Analysis** – monotonicity classification across datasets
4. **Trajectory Analysis** – anchored min-max normalization, NCL projection

## Contact
Kyungdo Kim, kkim207@jh.edu  
Johns Hopkins University School of Medicine
