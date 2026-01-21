# NCF2_EMT_heatmap
This repository contains the code used to generate Supplementary Figure 7 in "NRF2 activation by myeloid cell-derived oxidative stress induces SNAI-driven EMT and metastasis in breast cancer" by M. Kaya et al.

## Requirements
- R (>= 4.2 recommended)
- Packages: pheatmap, RColorBrewer

## Run
1. Open `260121 Heatmap for publication.Rmd` in RStudio
2. Put the expression table at: `data/expression.txt` (see below)
3. Knit, or run chunks sequentially

## Data
The data was accessed from https://www.cbioportal.org/study/summary?id=brca_tcga_pan_can_atlas_2018 in November 2023. Genes included are from “HALLMARK_EPITHELIAL_MESENCHYMAL_TRANSITION” (M5930) and “SARRIO_EPITHELIAL_MESENCHYMAL_TRANSITION_DN” (M11513), together with 24 additional genes of interest (GOI) that are denoted according to typical epithelial phenotype (“E+”), mesenchymal phenotype (“M+”), or “other” (Supplementary Table S5). Duplicate genes were excluded. NCF2 was included to sort patients according to NCF2-expression, but was excluded from the expression matrix that the heatmap was based upon. "mRNA expression z-scores relative to all samples (log RNA Seq V2 RSEM)" was downloaded.

The dataset is publicly available via cBioPortal. Please cite cBioPortal and the original data source as required by the dataset’s terms.

## Output
- `NCF2_heatmap_A4_300dpi.tiff`
- `NCF2_heatmap_A4.pdf`
