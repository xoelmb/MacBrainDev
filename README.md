# MacaqueDev2023

This repository contains code for reproducing the figures 7A and B, and supplementary 16A, B and C in the publication:


Nicola Micali *et al.*, **Molecular programs of regional specification and neural stem cell fate progression in macaque telencephalon**. *Science* **382**, eadf3786 (2023). DOI:10.1126/science.adf3786


# Description

- `notebooks/`
  - `1.EWCEanalysis.ipynb`: contains code to perform EWCE analysis, including finding marker genes, SCT-normalization and CellTypeData object.
  - `2.EWCEresults.ipynb`: contains code to reproduce the figures 7A and supplementary 16A in the publication.
  - `3.MarkersAndExpressionData.ipynb`: contains helper functions to gather expression summaries of defined groups of cells, including finding marker genes, scaling expression and gathering expression averages. Used in following figures.
  - `4.DiseaseExpressionInPCs.ipynb`: contains code to gather expression data from disease genes and plot it in the different subsets of the data. It also compares markers and disease genes to compute the fisher test of the overlaps, and contains functions to plot it (Figure S16B).
  - `5.PCmarkers.ipynb`: the code plots the expression of Patterning center marker genes in the whole data. The genes are also prioritised to those the least expressed in other cell types of the neural lineage or early timepoints (figure 7C and S16C).

- `raw/`: contains input files, specifically:
  - `All.MNN.v1.org.rds`*: expression dataset from the study
  - `all.nhp.cbn.v6.txt`: cell class and subtype information
  - `Patterning_center_cluster_order.tsv`: groups of Patterning center subtypes to use
  - Sets of disease-associated genes

- `data/`: contains intermediate and processed files produced by the notebooks. 


`*` contact me or the corresponding authors of the study to request access to the expression dataset.