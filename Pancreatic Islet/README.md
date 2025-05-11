# Pancreatic Islet Cell Type Identification

## Project Description

This project analyzes single-cell RNA sequencing (scRNA-seq) data from human pancreatic islets to identify cell types and their marker genes. The dataset is from the GSE84133 study available on GEO. The primary goal is to classify the different endocrine cell types within the islets, such as alpha, beta, delta, and PP cells.

## Approach

The analysis follows these steps:

1. **Data Loading and Preprocessing:**
    - Download the raw data from GEO and load it into an AnnData object using Scanpy.
    - Filter out cells with low gene counts and genes expressed in few cells.
    - Remove cells with high mitochondrial content, which can indicate low quality or dying cells.
    - Normalize gene expression and transform to log counts for better comparability.
2. **Dimensionality Reduction and Clustering:**
    - Identify highly variable genes, which are likely to be informative for cell type differences.
    - Perform Principal Component Analysis (PCA) to reduce the dimensionality of the data while retaining important information.
    - Compute a neighborhood graph for cells based on their PCA coordinates, representing their similarity.
    - Perform Uniform Manifold Approximation and Projection (UMAP) to visualize the cells in a two-dimensional space.
    - Cluster cells using the Leiden algorithm to group similar cells together.
3. **Cell Type Annotation:**
    - Identify marker genes for each cluster using differential gene expression analysis.
    - Use known marker genes for pancreatic islet cell types to annotate clusters, assigning them to specific cell types.
    - Visualize the annotated cell types on the UMAP plot to see their distribution and relationships.

## Dependencies

- Python 3.7 or higher
- Scanpy
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Leidenalg

## Results

The analysis identifies several distinct cell types within the human pancreatic islets, including alpha, beta, delta, and PP cells. It also identifies marker genes for each cell type. The results are visualized using UMAP plots, showing the spatial organization of the cell types within the islets.
