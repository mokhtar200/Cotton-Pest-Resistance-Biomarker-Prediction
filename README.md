# Cotton Pest Resistance Biomarker Prediction

## Overview
This project aims to identify genetic markers associated with pest resistance in cotton plants. By analyzing gene expression data from cotton infected with the bollworm pest, a predictive model is built to classify cotton plants as resistant or susceptible to pest damage. The model is constructed using a machine learning approach (Random Forest) and identifies the most important genes (biomarkers) for pest resistance. Gene Ontology (GO) enrichment analysis is also performed to understand the biological functions of these markers.

## Data Source:
- **Dataset**: [GSE106409](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE106409) – Gene expression data for cotton infected by the bollworm pest.
- **Organism**: Cotton (Gossypium hirsutum).
- **Data Type**: Gene expression data.
- **Condition**: Infected with bollworm, focusing on pest resistance in cotton plants.

## Goals:
1. **Data Preprocessing**: Clean and preprocess gene expression data for downstream analysis.
2. **Feature Selection**: Identify variable genes associated with pest resistance using statistical methods.
3. **Model Building**: Train a predictive model (Random Forest) to classify cotton plants as resistant or susceptible to pests.
4. **Marker Identification**: Identify genetic markers (genes) associated with pest resistance.
5. **Gene Ontology (GO) Enrichment**: Perform GO enrichment analysis on the important genes to explore their biological relevance.
6. **Model Evaluation**: Assess model performance using ROC curve and feature importance.

## Prerequisites:
1. R version 3.6 or higher.
2. Required R packages:
    - `GEOquery` - For downloading data from GEO.
    - `Seurat` - For gene expression analysis and clustering.
    - `randomForest` - For machine learning model.
    - `ROCR` - For performance evaluation.
    - `caret` - For data partitioning and model evaluation.
    - `clusterProfiler` - For gene ontology enrichment analysis.
    - `ggplot2` - For visualization.

To install the required R packages, run the following code in R:

```R
install.packages(c('GEOquery', 'Seurat', 'randomForest', 'ROCR', 'caret', 'clusterProfiler', 'ggplot2'))
