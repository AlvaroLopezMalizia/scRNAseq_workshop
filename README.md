# scRNAseq_workshop: Single Cell RNA Sequencing Analysis 🧬

Bioinformatic analysis of single cell RNA sequencing data applied to immunology
Universidad San Sebastián, Santiago, Chile

## Author
- **Name:** Joshua Waterfall
- **Affiliation:** Inserm U830 and Translational Research Dept, Institut Curie
- **Date:** November 2022

# Description added

## scRNASeq Analysis 📊
This serves as an introduction to analyzing single-cell RNA-seq (scRNAseq) data, with a focus on introduction. It primarily serves as a confidence-building exercise to gain experience with fundamental steps such as QC, normalization, dimensionality reduction, visualization, and sample merging. The primary tools used include the Seurat package by Rahul Satija's group, along with general methods from the tidyverse and the clustree package by Luke Zappia. While there are many other excellent tools available, these cover the needs of our workshop, are widely used, and nicely maintained.

## Key Differences in scRNASeq Analysis:
### 1- Sparse Data: 
scRNAseq data is sparse, with many more zeroes compared to bulk RNAseq data. This necessitates adjustments in statistical models and complicates drawing conclusions about individual genes in single cells.
### 2- Unsupervised Analysis:
Given the absence of labels or annotations for individual cells, unsupervised analysis is central in scRNAseq from the beginning.
### 3- Nonlinear Dimensionality Reduction:
With a vast number of cells in typical scRNAseq datasets, nonlinear dimensionality reduction techniques are crucial.

## Dataset Information:
- **Dataset:** 10X scRNAseq data from human PBMCs
- **Publication:** Kang, HM, et al, 2018 Nat Biotechnol.
- **Accession ID:** GSE96583 in NCBI GEO database

## Initial Setup:
To begin, create a new folder named "KangHM_2018_data" and a subfolder within it named "GSM2560245". Download the following files to the "GSM2560245" folder:
- Gene annotations: GSE96583_batch1.genes.tsv.gz
- Table of cells by genes: GSM2560245_A.mat.gz
- Cell barcodes: GSM2560245_barcodes.tsv.gz
