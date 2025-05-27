# scRNAseq_Tutorial

## Overview  
This repository contains an R Markdown-based tutorial workflow for single-cell RNA sequencing (scRNA-seq) data analysis. The workflow covers key steps such as quality control, normalization, batch effect correction using Harmony, clustering, and cell type annotation using SingleR.

The tutorial is designed to guide users through a reproducible scRNA-seq analysis pipeline built primarily with the Seurat package in R.

## About This Workflow

I developed and integrated this tutorial to create a comprehensive, reproducible scRNA-seq analysis pipeline. While the methods and tools (like Seurat, Harmony, and SingleR) come from publicly available tutorials and resources, this repository represents my own effort to combine these approaches into an end-to-end workflow applied to real single-cell data.

I adapted, tested, and documented the pipeline to make it user-friendly and practical for students and researchers new to single-cell RNA-seq analysis.

My goal is to provide a clear, well-organized guide that brings together existing tutorials into one cohesive workflow, supporting learning and reproducible research.

If you use or adapt this workflow, please give credit to this repository.


## Features  
- Data Quality Control (QC) and filtering  
- Data normalization and scaling  
- Batch effect correction with Harmony integration  
- Dimensionality reduction (PCA, UMAP)  
- Clustering of cells  
- Automated cell type annotation with SingleR  
- Fully reproducible analysis using R Markdown  

## Requirements  
- R (version >= 4.0)  
- R packages: Seurat, Harmony, SingleR, and dependencies (see tutorial for details)

## Data Source

The dataset used in this tutorial was obtained from a publicly available single-cell RNA-seq study on breast cancer:

**Luo L., Yang P., Mastoraki S., et al.**  
*Single-cell RNA sequencing identifies molecular biomarkers predicting late progression to CDK4/6 inhibition in patients with HR+/HER2- metastatic breast cancer.*  
**Molecular Cancer**, 2025.  
PMID: [39955556](https://pubmed.ncbi.nlm.nih.gov/39955556/) | PMCID: [PMC11829392](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC11829392/) | DOI: [10.1186/s12943-025-02226-9](https://doi.org/10.1186/s12943-025-02226-9)

The raw data is available through the Gene Expression Omnibus (GEO):  
**GEO Series Accession**: [GSE262288](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE262288)

For this tutorial, two samples were used:
- **GSM8162620** — Patient 3 ascites scRNA-seq sample 1  
- **GSM8162621** — Patient 3 ascites scRNA-seq sample 2  

These samples were selected to demonstrate the functionality of the workflow.

## Data Download

Due to file size limits, the raw scRNA-seq data matrices for samples GSM8162620 and GSM8162621 are **not included** in this repository.

Please download the data directly from the Gene Expression Omnibus (GEO) at:

- [GSM8162620 - Patient 3 ascites scRNA-seq sample 1](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSM8162620)
- [GSM8162621 - Patient 3 ascites scRNA-seq sample 2](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSM8162621)

For this tutorial, each sample's data should be stored in its own separate folder.

**Note:** You can organize these folders as you prefer, but make sure to update the file paths accordingly in the `tutorial.Rmd` script before running the analysis.

## How to Use  
1. Clone or download this repository.  
2. Open `tutorial.Rmd` in RStudio.  
3. Follow the code chunks and comments to run the analysis step-by-step.  
4. Install any missing packages as prompted.

## Acknowledgments

This tutorial was developed by adapting and integrating several excellent publicly available resources, including:  

- [Seurat PBMC 3k Tutorial](https://satijalab.org/seurat/articles/pbmc3k_tutorial.html) for the initial QC, normalization, and clustering steps.  
- [Harmony vignette for Seurat](https://cran.r-project.org/web/packages/harmony/vignettes/Seurat.html) for batch effect correction using Harmony.  
- [SingleR Tutorial by BioStatSquid](https://biostatsquid.com/singler-tutorial/) for automated cell type annotation.

I thank these authors for making their work openly accessible, which helped me build this integrated workflow.
Thanks to AI assistance for brainstorming and polishing ideas

## License  
This tutorial is licensed under the [MIT License](LICENSE). You are free to use, modify, and distribute this work, provided appropriate credit is given to the author.  

## Citation  
This workflow and tutorial were developed by Sai Harshitha Muddamsetty, 2025. Please cite or credit this repository if you use or adapt this work in your research or teaching.

---
## Contact

For questions, feedback, or collaboration, feel free to reach out:

- Email: harshithamuddamsetty@gamil.com  
- GitHub: [Harshitha-MI](https://github.com/Harshitha-MI)

If you have questions or feedback, please feel free to open an issue or contact me.

---

**Happy analyzing!**  
Harshitha

