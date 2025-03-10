# RRHO2-Analysis-of-Differential-Gene-Expression

## Overview
This project performs **Rank-Rank Hypergeometric Overlap (RRHO2)** analysis on gene expression data to compare **wild-type (WT)** and **HuR knockout (KO)** conditions. The analysis helps visualize gene expression similarities and differences between the two datasets.

## Project Structure
```
RRHO2_analysis/
│-- WT_E20_vs_WT_DMSO_deseq2.xls            # Wild-type gene expression ranking
│-- HuRKO_E20_vs_HuRKO_DMSO_deseq2.xls  # HuR knockout gene expression ranking
│-- RRHO2_WT_vs_HuR.tiff                    # Output heatmap image
│-- RRHO2_analysis.Rmd                      # RMarkdown script for analysis
```

## Requirements
Ensure you have the following R packages installed:
```r
install.packages("tidyverse")
install.packages("readxl")
install.packages("RRHO2")
```

## Expected Output
- **RRHO2_WT_vs_HuR.tiff**: A heatmap showing gene expression overlap patterns.

## Contact
For questions or issues, feel free to open an issue on GitHub.
