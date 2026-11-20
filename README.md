# Uncovering enhancers and super-enhancers implicated in stromal cell  activation using induced Pluripotent Stem Cells-TGFB1 kidney derived organoids a model of kidney fibrosis
The epigenetic regulation has emerged as an important mechanism through which extracellular injury signals may be translated into sustained changes in gene expression and cellular behaviour. My aim is to understand the epigenetic landscape driving the expression of ECM genes implicated in fibrosis and provide a computational analysis of putative loci for CRISPRi for functional validation. We aim that this loci can reduce the ECM turn over with therapeutic value and ameliorate CKD.

## Analysis of scRNA-seq dataset in [seurat](https://satijalab.org/seurat/)
1. Quality control, normalisation, clustering and annotation of control & tgb1 treated iPSCs-kidney derived organoid.
2. Sub-clusting of fibroblast population & comparative analysis with existing kidney patient datasets [CKD patient data ](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE211785) & [ECM-receptor data](https://www.kegg.jp/pathway/hsa04512)

      <img width="453" height="301" alt="image" src="https://github.com/user-attachments/assets/93279d09-4398-4596-84f8-c10108c10f0f" />
  
## Analysis of scATAC-seq dataset in [signac](https://stuartlab.org/signac/)
1. Quality control, clustering and dimensionality reduction.

2. Gene activity analysis & anchor identification for CCA integration.

3. DIfferential accesibility analysis between (Fibroblast ~ Myofibroblast) to infer putataive regulatory regions.

3. Linkage analysis to predict gene-cis regulatory interaction using [cicero](https://github.com/cole-trapnell-lab/cicero-release).

   <img width="435" height="572" alt="image" src="https://github.com/user-attachments/assets/8ac19e61-203c-4d88-99c6-afe7a6370f15" />

## Enhancer and super-enhancer ranking and annotation using ([ROSE](https://github.com/stjude/ROSE) & [GREAT](https://great-help.atlassian.net/wiki/spaces/GREAT/overview))

1. Motif enrichment analyis to infer SMAD3 TF enriched regions using [Homer](http://homer.ucsd.edu/homer/).

2. Comparative validataion of identified putative enhanncers using [Encode](https://genome.ucsc.edu/cgi-bin/hgTracks?db=mm10&lastVirtModeType=default&lastVirtMode) fibroblast chip-seq,HI-C datasets (H3K27ac,H3K4Me1,CTCF & REMAP TF).

<img width="453" height="247" alt="image" src="https://github.com/user-attachments/assets/54815aa5-4653-472d-8188-23dd6501b452" />

# R package installation guide for reproducible analysis

This  instructions for installing  bioinformatics and visualization R packages used in scRNA-seq and data visualization.

## Installation instructions

You can install the packages directly from CRAN or Bioconductor, or from GitHub where applicable.

### Install from CRAN

Open  R console or RStudio and run:

```r
install.packages(c("patchwork","Signac","cowplot","Seurat","sctransform","glmGampoi","DoubletFinder", "monocle3", "pheatmap", "ggplot2", "ggvennDiagram"))
