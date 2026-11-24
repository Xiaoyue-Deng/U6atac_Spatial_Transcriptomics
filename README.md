# Repository Catalogue
This repository contains code used for Nanostring GeoMx analysis. 
The main script used for the manuscript is under the same repository, while supporting scripts on spatial deconvolution can be found in the [support_scripts](https://github.com/Xiaoyue-Deng/Spatial_Transcriptomics/tree/main/support_scripts).

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
