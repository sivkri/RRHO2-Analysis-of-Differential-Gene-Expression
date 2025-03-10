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
install.packages(c("dplyr", "ggplot2", "grid", "readxl","tidyverse", "devtools"))
# Install RRHO2 separately
devtools::install_github("yah2012/RRHO2")
```
## Data

Place the following files in the working directory:

- `wt_treatment_effect_deseq2_annotated.xls`
- `abi1_treatment_effect_deseq2_annotated.xls`

## Usage

Run the analysis using the provided RMarkdown (`.Rmd`) file:

1. Open `analysis.Rmd`
2. Execute code chunks or knit to an HTML report

Alternatively, run it as a standalone R script:

```r
rmarkdown::render("analysis.Rmd")
```

## Expected Output
- **Venn Diagram & Heatmap:** Visualizing overlap between WT and ABI1.
- **Summary Statistics:** Gene overlap and correlation analysis.
- **TIFF Image:** `RRHO2_wt_abi1.tiff` (for publication-ready visuals).


## Contact
For questions or issues, feel free to open an issue on GitHub.
