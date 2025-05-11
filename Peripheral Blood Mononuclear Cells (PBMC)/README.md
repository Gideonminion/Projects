# Single-cell RNA Sequencing Analysis of PBMC3k Dataset using Scanpy

## Project Description

This project aims to analyze the PBMC3k dataset, a publicly available single-cell RNA sequencing (scRNA-seq) dataset of peripheral blood mononuclear cells (PBMCs), using the Scanpy library in Python. The analysis includes quality control, normalization, dimensionality reduction, clustering, and identification of marker genes for cell type annotation. Additionally, the project explores trajectory inference using scVelo to understand the dynamic processes within the cells.

## Approach

The analysis workflow follows these key steps:

1. **Data Loading and Quality Control:**
    - Load the PBMC3k dataset using Scanpy's built-in function.
    - Perform quality control to remove low-quality cells and genes based on metrics such as the number of genes detected, total counts, and mitochondrial gene expression.

2. **Normalization and Feature Selection:**
    - Normalize the data to account for differences in sequencing depth between cells.
    - Identify highly variable genes, which are likely to be informative for downstream analysis.

3. **Dimensionality Reduction and Clustering:**
    - Reduce the dimensionality of the data using Principal Component Analysis (PCA).
    - Cluster the cells using the Leiden algorithm to identify distinct cell populations.

4. **Marker Gene Identification and Cell Type Annotation:**
    - Identify marker genes for each cluster using differential expression tests (t-test and Wilcoxon rank-sum test).
    - Annotate the clusters based on the expression of known marker genes.

5. **Trajectory Inference:**
    - Utilize scVelo to perform RNA velocity analysis and infer the developmental trajectories of cells.
    - Identify genes and pathways associated with cell fate transitions.

## Dependencies

- Python 3.x
- Scanpy
- scVelo
- NumPy
- Pandas
- Matplotlib
- leidenalg

## Results

The analysis identified distinct cell populations within the PBMC3k dataset, including CD4 T cells, CD8 T cells, B cells, NK cells, monocytes, and dendritic cells. Marker genes for each cluster were identified and used for cell type annotation. Trajectory inference revealed potential developmental pathways and dynamic processes within the cells.

## Conclusion

This project explores the application of Scanpy and scVelo for analyzing scRNA-seq data. The results provide insights into the cellular composition and dynamic behavior of PBMCs, which can be further explored for understanding immune responses and disease mechanisms.
