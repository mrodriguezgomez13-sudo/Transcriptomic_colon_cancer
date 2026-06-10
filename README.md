
# RNA-seq colorectal cancer analysis

This project analyzes gene expression data obtained from RNA sequencing (RNA-seq) in patients with colorectal cancer (:contentReference[oaicite:0]{index=0}).  

The dataset is provided as a preprocessed `SummarizedExperiment` object and is based on the public GEO study series :contentReference[oaicite:1]{index=1}, available in the NCBI Gene Expression Omnibus (GEO) database.

The main objective is to study differential gene expression between normal tissue, primary tumor, and liver metastasis.


## Workflow

The analysis includes: 

- Data exploration and quality control (PCA, clustering, boxplots)
- Filtering of lowly expressed genes
- Normalization using TMM (edgeR)
- Differential expression analysis using limma-voom
- Functional enrichment analysis (GO) using clusterProfiler

## Requirements
R >= 4.x
- Bioconductor packages:
  - SummarizedExperiment
  - edgeR
  - limma
  - clusterProfiler
  - org.Hs.eg.db
  - factoextra
  
Main results

- Clear separation between sample types in PCA analysis
- Identification of differentially expressed genes between tumor and normal tissue
- Functional enrichment of biological processes related to cancer progression

## How to run
Open `report.Rmd` and knit to HTML.
