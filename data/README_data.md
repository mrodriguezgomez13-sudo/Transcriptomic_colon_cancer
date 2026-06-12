# Data

The raw data file (`PEC2_GSE50760_colorectal_SE.Rda`) is not included in this repository.

## How to obtain the data

The analysis is based on the public GEO series **GSE50760**:

> Kim S.K. et al. (2014). A nineteen gene-based risk score classifier predicts prognosis of colorectal cancer patients. *Molecular Oncology*, 8(8), 1653–1666.

### Direct download from GEO

1. Go to: https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE50760
2. Download the raw count matrix from the supplementary files section.

The script expects the file at this exact path:

```r
load("data/PEC2_GSE50760_colorectal_SE.Rda")
```