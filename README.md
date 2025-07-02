# scRNAseq_Tutorial  

## Overview  
This repository contains an **R Markdown-based tutorial workflow** for single-cell RNA sequencing (scRNA-seq) data analysis.

**scRNA-seq** is a powerful technique that enables the profiling of gene expression at the resolution of individual cells, offering insights into cellular heterogeneity, development, and disease mechanisms. For a deeper introduction, see:  
👉 [Single-cell transcriptomics: a review of applications and future perspectives (Haque et al., *Genome Medicine* 2017)](https://genomemedicine.biomedcentral.com/articles/10.1186/s13073-017-0467-4)

The workflow covers key steps such as:
- quality control (QC)
- normalization
- batch effect correction (using **Harmony**)
- clustering
- cell type annotation (using **SingleR**)

The tutorial guides users through a **reproducible scRNA-seq analysis pipeline**, built primarily with the **Seurat** package in R.

---

## About This Workflow  
I developed this tutorial to provide a clear, end-to-end, and reproducible scRNA-seq analysis pipeline. While the tools (Seurat, Harmony, SingleR) come from publicly available resources, this repository represents my effort to integrate, test, and document a cohesive workflow applied to real scRNA-seq data.

My goal is to support learning and reproducible research by offering a practical guide for students and researchers new to single-cell RNA-seq analysis.

➡ *If you use or adapt this workflow, please credit this repository.*

---

## Features  
✅ Data quality control and filtering  
✅ Data normalization and scaling  
✅ Batch effect correction using **Harmony**  
✅ Dimensionality reduction (PCA, UMAP)  
✅ Cell clustering  
✅ Automated cell type annotation with **SingleR**  
✅ Fully reproducible analysis using R Markdown  

---

## Requirements  
- **R** (version ≥ 4.0)  
- R packages: `Seurat`, `Harmony`, `SingleR`, and dependencies (see tutorial for installation details)

---

## Data Source  
This tutorial uses data from:

**Luo L., Yang P., Mastoraki S., et al.**  
*Single-cell RNA sequencing identifies molecular biomarkers predicting late progression to CDK4/6 inhibition in patients with HR+/HER2- metastatic breast cancer.*  
*Molecular Cancer, 2025.*  
PMID: 39955556 | PMCID: PMC11829392 | DOI: [10.1186/s12943-025-02226-9](https://doi.org/10.1186/s12943-025-02226-9)

**GEO accession:** [GSE262288](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE262288)

Samples used:
- GSM8162620 — Patient 3 ascites scRNA-seq sample 1
- GSM8162621 — Patient 3 ascites scRNA-seq sample 2  

*Note: These samples are treated as biological replicates for this tutorial, regardless of their original experimental context.*

---

## Data Download  
⚠ Due to file size limits, raw data matrices are **not included** in this repository.

👉 Download the data directly from GEO:
- [GSM8162620](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSM8162620)
- [GSM8162621](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSM8162621)

💡 Store each sample’s data in its own folder.  
Each folder should contain the following files (with exact names):
- `barcodes.tsv.gz`
- `features.tsv.gz`
- `matrix.mtx.gz`

➡ Ensure the file names match these conventions so the tutorial script can read them correctly. Update the file paths in `tutorial.Rmd` if your folder structure differs.


## How to Use  

### 1️⃣ Clone or download this repository  

#### MacOS / Linux (using Terminal)  
If you have **Git** installed:  
```bash
git clone https://github.com/Harshitha-MI/scRNAseq_Tutorial.git
Alternatively, download and unzip:

wget https://github.com/Harshitha-MI/scRNAseq_Tutorial/archive/refs/heads/main.zip
unzip main.zip
Windows

If you have Git Bash, use the same git clone command as above.
Or download the ZIP directly from GitHub and extract it using File Explorer.
2️⃣ Open tutorial.Rmd in RStudio
3️⃣ Follow the code chunks and comments step-by-step
4️⃣ Install any missing packages as prompted
Acknowledgments

This tutorial integrates concepts from:

Seurat PBMC 3k Tutorial (QC, normalization, clustering)
Harmony vignette for Seurat (batch correction)
SingleR Tutorial by BioStatSquid (cell type annotation)
Thanks to these authors for making their work publicly available. I also thank AI tools that assisted with brainstorming and polishing ideas.

License

This tutorial is licensed under the MIT License. You are free to use, modify, and distribute this work with appropriate credit to the author.

Citation

This workflow was developed by Sai Harshitha Muddamsetty, 2025.
➡ Please cite or credit this repository if you use or adapt this work in your research or teaching.

Contact

📧 harshithamuddamsetty@gmail.com
🐙 GitHub: Harshitha-MI

If you have feedback or questions, feel free to open an issue or contact me.

🌟 Happy analyzing!


