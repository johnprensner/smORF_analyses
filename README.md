# smORF_analyses
This repository provides additional details on the data analyses for gene expression studies after expression of smORFs in cancer cells.

## L1000 Data 

### Data availability

L1000 data can be found ??. 

### Data processing pipeline 

L1000 data were processed using the standard L1000 pipeline as described
in [Subramanian et al. 2017](https://pubmed.ncbi.nlm.nih.gov/29195078/).
Code for the pipeline itself is [here](https://github.com/cmap/cmapM). 

### Quality control 

Standard quality control was performed using the standard L1000 pipeline as
described in
[Subramanian et al. 2017](https://pubmed.ncbi.nlm.nih.gov/29195078/).
Code for the pipeline itself is [here](https://github.com/cmap/cmapM), and 
you can find more details about these methods
[here](https://clue.io/connectopedia/l1000_qc).

Additional custom quality control was also performed; code can be found
in `L1000/custom_smORF_L1000_QC.Rmd`.

### L1000 Signature generation

Signatures were generated using the standard L1000 pipeline as described
in [Subramanian et al. 2017](https://pubmed.ncbi.nlm.nih.gov/29195078/).
Code for the pipeline itself is [here](https://github.com/cmap/cmapM). 

### L1000 signature reproducibility and bioactivity

Measures of L1000 signature reproducibility and bioactivity (i.e.
transcriptional activity) were computed using the standard metric
generation approach described in
[Subramanian et al. 2017](https://pubmed.ncbi.nlm.nih.gov/29195078/).
The formulas used are listed in the smORF manuscript's methods section,
but you can also find more details and examples about these metrics
[here](https://clue.io/connectopedia/signature_quality_metrics).

### Visualization 

Standard `cmapR` was used for manipulating L1000 data files; you can
find the code for this [here](https://github.com/cmap/cmapR). Once in
tabular form, `tidyverse` was used to tabulate metrics and `pheatmap`
was used to generate clustered heatmaps. 


