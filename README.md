# Differential Expression Analysis in Colorectal Cancer (RNA-seq)

**Author:** Mònica Rodríguez Gómez  
**Course:** Anàlisi de dades òmiques — UOC  
**Date:** May 2026  
**Dataset:** [GSE50760](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE50760) (GEO/NCBI)

---

# RNA-seq colorectal cancer analysis

This project performs a complete RNA-seq differential expression analysis comparing **primary colorectal tumor tissue** vs. **normal colon tissue** in 10 paired patients.

The dataset is **not included** in this repository due to file size. It is based on the public GEO series **GSE50760**, which contains RNA-seq data from 54 samples (18 patients × 3 tissue types: normal colon, primary tumor, liver metastasis).

The analysis includes: 

- Exploratory data analysis (boxplots, PCA, hierarchical clustering, heatmaps)
- Filtering of low-expression genes and TMM normalization
- Differential expression analysis using `limma` + `voom` (paired design)
- Gene Ontology (GO) Over-Representation Analysis (ORA) for up- and down-regulated genes

## Main results

- Clear separation between sample types in PCA analysis
- Identification of differentially expressed genes between tumor and normal tissue
- Functional enrichment of biological processes related to cancer progression


## Requirements
Open R and run:

```r
install.packages("BiocManager")

BiocManager::install(c(
  "SummarizedExperiment",
  "edgeR",
  "limma",
  "clusterProfiler",
  "org.Hs.eg.db",
  "enrichplot"
))

install.packages(c("factoextra", "ggplot2"))
```

---

## License

This project is shared for academic purposes. The original dataset (GSE50760) is publicly available through NCBI GEO and subject to its own terms of use.
