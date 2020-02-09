UQ PhD Thesis Rmarkdown Template
========================

This repository provides a template for a University of Queensland PhD thesis using Rmarkdown with the bookdown package. It is designed for PhD students, but can be modified for Masters degrees and other universities as required.  The template is derived from ![Rob Hyndman's Monash Thesis Github repository](https://github.com/robjhyndman/MonashThesis) and also the ![Latex Overleaf](https://www.overleaf.com/edu/uq) template provided by the UQ Graduate School. 

## Requirements

To set up the software, you will need to install the `bookdown` package and its dependencies as follows:

```r
install.packages('bookdown')
```

You will also need LaTeX installed. If you don't already have LaTeX, one convenient approach is to install it via R:

```r
install.packages('tinytex')
tinytex::install_tinytex()
```
