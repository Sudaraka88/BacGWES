
<!-- badges: start -->

[![R](https://github.com/Sudaraka88/BacGWES/workflows/r.yml/badge.svg)](https://github.com/Sudaraka88/BacGWES/actions)
<!-- badges: end -->

# BacGWES

## Genomewide Epistasis Analysis on Bacteria

## Installation

`BacGWES` is currently available on github. It can be installed with
`devtools`

``` r
install.packages("devtools")
devtools::install_github("Sudaraka88/BacGWES")
```

## Quick Start

To run BacGWES, all you need is the fasta alignment and the
corresponding genbank annotation file.

``` r
# devtools::install_github("Sudaraka88/BacGWES")
library(BacGWES)
dset <- "spn23f_sample"
aln_path <- system.file("extdata", "sample_spn23f.aln", package = "fastbaps")
gbk_path <- system.file("extdata", "spn23f.gbk", package = "fastbaps")
BacGWES(dset = dset, aln_path = aln_path, gbk_path = gbk_path, SnpEff_Annotate = F)
```
