# INTRODUCTION

Using bulk RNA sequencing, we can pinpoint Differentially Expressed genes (DE genes) across replicates under varying conditions and proceed to their functional characterization. The data employed in this analysis is sourced from Recount3, a renowned repository for RNA-seq experiments. Comprehensive, unfiltered datasets from three human tissues - namely brain, pancreas, and kidney- were obtained for our study.

# QUALITY CONTROL

To ensure the accuracy of our study, we excluded samples that exhibited:

An RNA integrity number (RIN) exceeding 7.
A proportion of reads mapped to ribosomal RNA genes that surpassed 0.1.
A percentage of uniquely mapped reads falling below 85%.

# ANALYSIS

Count tables were established for each of the three tissues. Genes were then subjected to an expression-based filter, excluding those with nearly all 0 read counts. Subsequent normalization was achieved using the TMM (Trimmed Mean of M-values) method.

Through Multi Dimensional Scaling, we visualized a two-dimensional projection representing the distances between gene expression profiles. The aim here is to verify that replicates from identical tissues exhibit tight clustering.

To isolate significant DE genes, we undertook pairwise comparisons of gene expressions amongst the three tissues. Genes that displayed overexpression in one tissue relative to the other two were identified. The resultant lists were then refined based on the following statistical criteria:

FDR below 0.01.
logCPM exceeding 0.
Exclusion of genes with sparse or absent annotation.

# RESULTS

We identified genes for each tissue that were notably overexpressed in comparison to the other two tissues. Functional analysis underlined the reliability of the DE gene analysis results.
