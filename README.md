# Oak Microbiome Supplementary Material

This repository contains supplementary data and analysis scripts associated with the manuscript *"Beyond detection: Unveiling microbial dynamics in oak seedlings using isolation and HTAS."*

## 📂 Repository Structure

```
oak_microbiome_supplementary/
├── data/                # Pre-processed data subsets used for all analyses
│   ├── bacteria_OTU_table_subset.txt
│   ├── fungi_OTU_table_subset.txt
│   ├── diversity_indices_subset.txt
│   ├── soil_subset.txt
│   ├── matadata.txt
│   ├── funguild_*.txt
│   └── ...
├── scripts/             # Jupyter Notebooks used to perform the analysis
│   ├── diversity.ipynb
│   ├── funguild.ipynb
│   ├── soil.ipynb
│   └── cytoscape.ipynb
└── README.md            # This file
```

## 🔬 Contents

### `data/`
- Subset data tables derived from the full HTAS dataset, annotated fungal tables (FUNGuild), soil chemistry, diversity indices, and trophic group assignments.
- All files are tab-delimited `.txt` and can be imported directly into R, Python, or Cytoscape.

### `scripts/`
- Jupyter notebooks used in the analysis pipeline:
  - `diversity.ipynb`: Calculation of alpha diversity indices.
  - `funguild.ipynb`: Functional annotation and relative abundance of trophic groups.
  - `soil.ipynb`: Relationship between microbiome composition and soil properties.
  - `cytoscape.ipynb`: Generation of co-occurrence networks and Cytoscape export.

## 🧪 Methods Summary

- Microbial abundances were transformed using either TSS normalization (for diversity analyses) or CLR transformation (for correlation and network inference).
- Spearman correlation (|ρ| > 0.6, p < 0.05) was used to infer microbial co-occurrence networks.
- Functional annotations were obtained using FUNGuild and manually curated.
- Soil chemical properties were integrated as explanatory variables in ordination and correlation analyses.

## 📎 Citation

If you use this repository or data in your work, please cite:

> Frejlichová, L., et al. (2025). *Beyond detection: Unveiling microbial dynamics in oak seedlings using isolation and HTAS*. [Manuscript in review]

## 📝 License

This repository is shared for transparency and reproducibility. Please contact the author for permission before reusing data or scripts for other publications.
