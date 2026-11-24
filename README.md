# U6atac_Spatial_Transcriptomics Repository Catalogue
Code for the analysis of spatially resolved U6atac expression in advanced prostate cancer using NanoString GeoMx DSP. Associated with the manuscript
_"Inhibiting Minor Intron Splicing Disrupts DNA Repair and Sensitizes Hormone-Driven Tumors to Genotoxic Therapy"_ (submitted) and the master thesis _"Splicing Patterns and Spatially Resolved Characterization of U6atac Landscape in Advanced
Prostate Cancer"_.

---
## Workflow
1. `support_scripts/` – upstream processing of the GeoMx dataset
   (normalization comparison, spatial deconvolution, etc).
2. `DNA_repair_analysis.R` – differential expression and volcano plot
   used for the manuscript.

---

## 📦 Requirements

- R version: ≥ 4.2.0
- Recommended environment management: [renv](https://rstudio.github.io/renv/)
- Required R packages:
  - tidyverse
  - readxl
  - openxlsx
  - DESeq2
  - clusterProfiler
  - org.Hs.eg.db
  - enrichplot
  - EnhancedVolcano
  - pheatmap
  - ggrepel
  - sessioninfo

To install missing packages:

```r
install.packages(c("tidyverse", "readxl", "openxlsx", "ggrepel"))
BiocManager::install(c("DESeq2", "clusterProfiler", "org.Hs.eg.db",
                       "enrichplot", "EnhancedVolcano", "pheatmap"))

```

## Data availability
The raw and processed GeoMx data are not included in this repository (human patient data). 


## License
MIT.
