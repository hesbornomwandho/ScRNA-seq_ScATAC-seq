# Single cell multi-omics to uncover enhancers and super-enhancers  in stromal cell  activation using iPSCs-kidney derived organoid a model of kidney fibrosis


## Analysis of scRNA-seq dataset in [Seurat](https://satijalab.org/seurat/)

1. Quality control, normalisation, clustering and annotation of control & tgb1 treated ipscs-kidney derived organoid.

2. Sub-clusting of fibroblast population & comparative analysisi with existing kidney patient datasets [CKD patient data ](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE211785) & [ECM-receptor data](https://www.kegg.jp/pathway/hsa04512)

      <img width="453" height="301" alt="image" src="https://github.com/user-attachments/assets/93279d09-4398-4596-84f8-c10108c10f0f" />
  
## Analysis of chromatin accesibility (scATAC-seq) in [signac](https://stuartlab.org/signac/)

1. Quality control, clustering and dimensionality reduction.

2. Gene activity analysis & anchor identification for CCA integration.

3. DIfferential accesibility analysis between (Fibroblast ~ Myofibroblast) to infer putataive regulatory regions

3. Linkage analysis to predict gene-cis regulatory interaction using [cicero](https://github.com/cole-trapnell-lab/cicero-release)

   <img width="435" height="572" alt="image" src="https://github.com/user-attachments/assets/8ac19e61-203c-4d88-99c6-afe7a6370f15" />

## Enhancer and Super-enhancer ranking and annotation using ([ROSE](https://github.com/stjude/ROSE) & [GREAT](https://great-help.atlassian.net/wiki/spaces/GREAT/overview))

1. Motif enrichment analyis to infer SMAD3 TF enriched regions

2. Comparative validataion of identified putative enhanncers using Encode fibroblast chip-seq,HI-C dataset (H3K27ac,H3K4Me1,CTCF & REMAP TF)

<img width="453" height="247" alt="image" src="https://github.com/user-attachments/assets/54815aa5-4653-472d-8188-23dd6501b452" />


# R Package installation guide for reproducible

This  instructions for installing  bioinformatics and visualization R packages used in scRNA-seq and data visualization.

## Installation Instructions

You can install the packages directly from CRAN or Bioconductor, or from GitHub where applicable.

### Install from CRAN

Open your R console or RStudio and run:

```r
install.packages(c("patchwork","Signac","cowplot"," Seurat","sctransform", "DoubletFinder", "monocle3", "pheatmap", "ggplot2", "ggvennDiagram"))
