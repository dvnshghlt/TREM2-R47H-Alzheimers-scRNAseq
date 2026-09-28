# TREM2 R47H Single-Cell Alzheimer's Disease Atlas

## Overview

This project investigates cellular and functional changes associated with the
TREM2 R47H variant in an Alzheimer's disease single-cell RNA-seq dataset.

The analysis was performed using single-cell transcriptomic data to:

- Explore the cellular composition of the dataset
- Annotate major brain cell populations
- Compare TREM2 R47H and wild-type (WT) genotypes
- Identify cell-type-specific molecular changes
- Perform Gene Ontology (GO) enrichment analysis
- Perform ranked-gene Gene Set Enrichment Analysis (GSEA)
- Integrate cell-type and pathway-level findings into a biological interpretation

## Dataset

**Dataset:** GSE243292

**Input:** Single-cell RNA-seq dataset in `.h5ad` format

The original large `.h5ad` dataset is not included in this repository because
of its size. The analysis outputs and workflow are provided instead.

## Dataset Overview

- **Total cells:** 122,603
- **Genes:** 26,423
- **WT cells:** 92,324
- **TREM2 R47H cells:** 30,279

### Cell types identified

- Astrocytes (Ast)
- Endothelial cells (End)
- Excitatory neurons (Ex)
- Inhibitory neurons (In)
- Microglia (Mic)
- Oligodendrocytes (Oli)
- Oligodendrocyte precursor cells (Opc)

## Analysis Workflow

```text
Raw scRNA-seq dataset
        ↓
Data exploration & quality assessment
        ↓
Cell-type annotation
        ↓
UMAP visualization
        ↓
TREM2 genotype characterization
        ↓
R47H vs WT comparison
        ↓
Cell-type-specific analysis
        ↓
GO enrichment
        ↓
Ranked-gene GSEA
        ↓
Biological integration
## Key Results & Visualizations

### Cell-Type Annotation

UMAP visualization showing the major cell populations identified in the
single-cell dataset.

![Cell Type UMAP](notebooks/results/final_results/UMAP_final_celltype_annotation.png)

### TREM2 Genotype Distribution

UMAP visualization showing the distribution of TREM2 WT and R47H cells.

![TREM2 Genotype UMAP](notebooks/results/final_results/UMAP_TREM2_genotype.png)

### Cell-Type Composition

Comparison of WT and R47H cell-type composition.

![Cell Type Composition](notebooks/results/final_results/WT_vs_R47H_celltype_composition.png)

### GO Enrichment

Functional enrichment analysis across the annotated cell populations.

![GO Enrichment](notebooks/results/final_results/GO_enrichment_summary.png)

### Microglial GSEA

Ranked-gene GSEA highlights biological processes associated with TREM2 R47H
in microglia.

![Microglia GSEA](notebooks/results/trem2_DE/GSEA_Microglia_Clean/Microglia_GSEA_summary.png)

### Microglial Leading-Edge Analysis

Leading-edge genes associated with the enriched microglial pathways.

![Leading Edge Heatmap](notebooks/results/trem2_DE/GSEA_Microglia_Clean/Microglia_GSEA_leading_edge_heatmap.png)