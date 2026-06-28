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
| `ProblemSet1.Rmd` | Biological sequence analysis using yeast open reading frame (ORF) sequences and chromosome-size data. The analysis proceeds from FASTA import and genome-scale summaries to ORF-level feature extraction, including GC content, coding-sequence translation, and amino-acid composition analysis. | Biological sequence analysis; FASTA handling; R/Bioconductor |
| `ProblemSet2.Rmd` | Sequence comparison and k-mer analysis across protein and DNA sequences. Amino-acid sequences are compared using Hamming distance, while DNA k-mer profiling is used to characterize repeat motifs, including telomeric-repeat patterns. | Sequence comparison; k-mer analysis; motif/repeat analysis |
| `ProblemSet3.Rmd` | Pairwise sequence alignment and sequencing-read simulation. Global and local alignment with substitution-matrix scoring are applied to detect protein-domain similarity, followed by simulation of chromosome-derived short reads with base-substitution errors. | Pairwise sequence alignment; protein-domain search; short-read simulation |
| `ProblemSet4.Rmd` | Genomic interval analysis of promoter, CpG island, and repeat-annotation tracks from the human genome. Overlap-based annotation is used to characterize promoter-associated CpG islands and repeat families, with Markov-model simulation and sliding-window CpG profiling used to examine regulatory-sequence composition. | Genomic interval analysis; regulatory sequence annotation; genome track analysis |
| `ProblemSet5.Rmd` | Gene-model annotation and genome organization across human gene biotypes. The analysis builds annotation resources from GTF data, summarizes protein-coding gene and exon structure, analyzes promoter sequence composition, and compares GC content across coding and noncoding genes. | Gene-model annotation; Ensembl BioMart; genomic feature analysis |
| `ProblemSet6.Rmd` | Case-control genetic association analysis and functional annotation of candidate variants. The workflow moves from genotype-frequency testing and multiple-testing correction to SNP-gene overlap analysis, coding-region annotation, and trait-focused variant-to-gene interpretation using GWAS Catalog data. | Genetic association analysis; GWAS annotation; variant-to-gene mapping |
| `ProblemSet7.Rmd` | RNA-seq experimental design and upstream processing for differential expression studies. The work links study design with RNA quality assessment, read quality control, splice-aware alignment, gene-level read summarization, and GTF/BED annotation handling. | RNA-seq experimental design; NGS preprocessing workflow; gene-level quantification |
| `ProblemSet8.Rmd` | RNA-seq normalization and sample-level quality assessment using gene-count data and genome annotation. The analysis filters low-information gene classes, recalculates TPM values, constructs a DESeq2 dataset, compares normalized and rlog-transformed counts, and interprets MA/PCA diagnostics for replicate assessment. | RNA-seq normalization; sample-level QC; DESeq2 count-data analysis |
| `Project2.Rmd` | Focuses on end-to-end bulk RNA-seq differential gene-expression analysis of mouse neural differentiation. The project moves from count-matrix and sample-metadata quality control to normalization, PCA-based sample assessment, differential expression testing, expression-pattern clustering, and GO over-representation analysis to interpret transcriptional programs during neural development. | Bulk RNA-seq analysis; differential gene-expression analysis; functional enrichment analysis |

## 4. R Dependencies

Dependencies:

- CRAN: `cluster`, `ggplot2`, `gridExtra`, `moments`, `pheatmap`, `scales`, `stringr`, `xtable`
- Bioconductor: `Biostrings`, `DESeq2`, `GenomicFeatures`, `biomaRt`, `clusterProfiler`, `gwascat`, `org.Mm.eg.db`, `pwalign`, `rtracklayer`

Install Bioconductor packages with `BiocManager`.

