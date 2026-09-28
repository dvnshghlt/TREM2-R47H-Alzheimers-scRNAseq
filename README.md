# TREM2 R47H Single-Cell Alzheimer's Disease Atlas

## Overview

This project investigates cellular and functional changes associated with the TREM2 R47H variant in an Alzheimer's disease single-cell RNA-seq dataset.

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

The original large `.h5ad` dataset is not included in this repository because of its size. The analysis outputs and workflow are provided instead.

## Dataset Overview

- **Total cells:** 122,603
- **Genes:** 26,423
- **WT cells:** 92,324
- **TREM2 R47H cells:** 30,279

### Cell Types Identified

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