# YSC3241 Computational and Systems Biology

![Computational Biology](images.jpeg)

## 1. Overview

This repository contains original solutions to problem sets and projects from YSC3241 Computational and Systems Biology, covering core bioinformatics workflows for genomic sequence analysis, genome annotation, gene-trait association analysis, and bulk RNA-seq differential gene-expression analysis.

## 2. Repository Structure

```text
.
├── problem-sets/          # Problem set R Markdown
│   └── rendered/          # Problem set HTML outputs
├── projects/              # Project R Markdown 
│   └── rendered/          # Project HTML outputs
├── data/                  # Datasets grouped by assignment or shared use
└── README.md
```

## 3. Files Summary

| File | Description | Relevant concepts |
| --- | --- | --- |
| `ProblemSet1.Rmd` | Analysis of open reading frames (i.e. protein coding regions) in the yeast genome. Characterization of ORF sizes and GC content. Transcription and translation of ORFs to amino acid sequences and analysis of amino acid composition.| Characterization of biological sequences |
| `ProblemSet2.Rmd` | Sequence alignment. Quantifying differences between DNA sequences and between amino acid sequences using Hamming distance. Application of DNA k-mer profiling to characterize repeat motifs (e.g. telomeric repeats) which result in mapping ambiguity in sequence alignment. | Sequence alignment |
| `ProblemSet3.Rmd` | Sequence alignment and genome assembly. Global alignment of genome sequences. Local alignment with applications to homeobox domain detection in amino acid sequences. Simulation of short-read genome sequencing with and without base-substitution errors. | Sequence alignment and genome assembly |
| `ProblemSet4.Rmd` | Genome annotation. Characterisation of genomic regions such as promoters and their overlap with CpG islands and other repeat elements. Application of hidden markov models to model the genome as a sequence of "observable" events (like DNA bases A, T, C, G) that depend on "hidden" underlying states (like exons, introns, or promoters).| Genome annotation |
| `ProblemSet5.Rmd` | Genome annotation. Characterisation of protein-coding regions, with a focus on exons and GC content. | Genome annotation |
| `ProblemSet6.Rmd` | Genetic variation. Identification of genomic variants (SNPs) significantly associated with a trait (case vs control) in a simulated genome-wide association study (GWAS). Interpretation of genomic variants by variant-to-gene and gene-to-trait mapping. | GWAS and variant interpretation |
| `ProblemSet7.Rmd` | RNA Sequencing. RNA-Seq experiment design. Exploration of genome annotation file formats (gtf). Characterization of RNA-Seq raw counts data.| Bulk RNA-seq experiments|
| `ProblemSet8.Rmd` | Processing of RNA-Seq raw counts data. Plots for comparison of biological and technical replicates in RNA-Seq experiments.| Bulk RNA-seq data processing |
| `Project2.Rmd` | Bulk RNA-Seq data analysis. RNA seq data quality control, data processing, differential expression analysis, expression-pattern clustering, and GO over-representation analysis to interpret transcriptional programs involved in neural development.| Bulk RNA-seq data analysis |

## 4. R Dependencies

Dependencies:

- CRAN: `cluster`, `ggplot2`, `gridExtra`, `moments`, `pheatmap`, `scales`, `stringr`, `xtable`
- Bioconductor: `Biostrings`, `DESeq2`, `GenomicFeatures`, `biomaRt`, `clusterProfiler`, `gwascat`, `org.Mm.eg.db`, `pwalign`, `rtracklayer`

Install Bioconductor packages with `BiocManager`.

