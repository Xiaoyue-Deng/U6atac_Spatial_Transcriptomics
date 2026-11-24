# U6atac_Spatial_Transcriptomics Repository Catalogue
Code for the analysis of spatially resolved U6atac expression in advanced prostate cancer using NanoString GeoMx DSP. Associated with the manuscript
_"Inhibiting Minor Intron Splicing Disrupts DNA Repair and Sensitizes Hormone-Driven Tumors to Genotoxic Therapy"_ (submitted) and the master thesis _"Splicing Patterns and Spatially Resolved Characterization of U6atac Landscape in Advanced
Prostate Cancer"_.

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

## Notes on the script
`DNA_repair_analysis.R` is an exploratory analysis script. Several gene lists
and sections were run in parallel sessions, and only this script is reported
here. Some objects and input files referenced in it (e.g. gene list files,
`dds_tme`, `old_mig`) are therefore not defined in the script or not included
in this repository, and some sections cannot be run as provided. The script is
shared for transparency of the analysis used for spatial transcriptomic data analysis focusing DNA repair genes.

## License
MIT.
