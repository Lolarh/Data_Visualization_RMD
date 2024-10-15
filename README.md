
# TCGA Data Visualization Project

This project focuses on visualizing expression data from **The Cancer Genome Atlas (TCGA)** and additional datasets for genome annotation and differential gene expression analysis. The visualizations were created using R, and the aim is to illustrate how different types of data, such as gene expression levels, genomic annotations, and RNA-seq analysis results, can be effectively visualized for exploratory analysis.

## How to Access the Project

The detailed R code and visualizations can be accessed in the R Markdown file in the repository. Additionally, the rendered HTML version of the project can be viewed [here](https://lolarh.github.io/Data_Visualization_RMD/DA_dataViz.html)

---

## Data Overview

### 1. TCGA Expression Data

**The Cancer Genome Atlas (TCGA)** is a comprehensive resource containing genetic data related to cancer. This project works with two datasets: `tcga_cancer.csv` (containing gene expression data) and `tcga_cancer_labels.csv` (containing class labels). The first 200 samples for genes 1 to 43 were used for visualization.

### 2. GENCODE Human Genome Annotations

**GENCODE** provides detailed annotations of human genes. For this project, the `hg38_genes.tsv` file was used, containing 20,000 randomly selected annotated genes from the GENCODE dataset for the human genome (hg38). Genes were filtered based on their type and length, and then categorized for analysis and visualization.

### 3. Differential Gene Expression (DGE) Analysis

DGE is crucial for understanding gene activity under different conditions. The dataset `deseq2_dummy.txt` contains test results for 5000 genes obtained from a DGE analysis using the DESeq2 package. The top 2000 genes (based on normalized RNA-seq counts) were selected for visualization.

---

## Visualizations

### 1. Expression Distribution of Gene1

- **Histogram**: A histogram visualizes the distribution of Gene1 expression values with varying bin widths to assess the optimal choice for data representation.

### 2. Gene Expression Correlation

- **Scatterplot with Linear Regression**: Correlation between Gene1 and Gene12 was analyzed with a scatterplot, featuring a regression line and Pearson correlation coefficient. 

### 3. Class Proportions

- **Stacked Bar Chart**: A bar chart visualizes the relative and absolute proportions of gene classes.

### 4. Combined Plots

- **Multiple Panel Figure**: All individual visualizations are combined into a single figure using a package from the course.

---

## Human Genome Annotations

### 1. Gene Count by Class

- **Bar Chart**: This plot shows the number of genes per class, including mRNA, lncRNA, and pseudogenes.

### 2. Length Distribution

- **Density Plot & Alternative Plot**: A density plot visualizes the gene length distribution across different classes, with vertical lines marking the median gene length.

---

## Differential Gene Expression Analysis

### 1. Volcano Plot

- **Volcano Plot**: This plot visualizes fold change against statistical significance, highlighting differentially expressed genes with significant log2 fold change. Genes with adjusted p-values below 0.1 are labeled, especially those with log2 fold change > 2.

### 2. Heatmap

- **Heatmap**: A heatmap shows the expression values for the 20 genes with the lowest adjusted p-values, illustrating patterns of gene activity.

---



