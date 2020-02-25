Unofficial UQ PhD Thesis Template for R Markdown
================================================

This repository provides a template for a University of Queensland PhD thesis using Rmarkdown with the bookdown package. It is designed for PhD or Masters students.  The template is derived from Rob Hyndman's Monash Thesis Github repository (https://github.com/robjhyndman/MonashThesis) and also the The University of Queensland Official Latex Template (https://my.uq.edu.au/node/1707/4#4) provided by the UQ Graduate School. 

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

Any LaTex packages required by the template will be download when the thesis is knitted for the first time.

## Instructions

Edit LaTexPackages.tex to include any additional LaTex packages that you require.

Edit the metadata in index.Rmd to populate the title page.

Edit 00-abstract.Rmd to add an abstract.

Edit 00-preliminary.Rmd to add the information required by UQ to the preliminary pages.  By default, instructions will be printed in the compiled thesis.  This can be turned off by setting params:instructions to FALSE in index.Rmd.

Edit _bookdown.yml to change the order in which .Rmd files are assembled into the final thesis. New chapters and appendicies may be added by inserting extra lines in the appropriate order using the chapter files as a guide.

Replace references/bibliography.bib with your reference file in Bibtex format.

Several examples are included in the examples directory.

By default, citations are numbered and are included in the bibliography in citation order. Edit lines 118-129 in uqthesis.cls to change to an APA style, author-date format.

To compile the thesis into a .pdf file, open index.Rmd in RStudio and click the Knit button.

## Rules for use of Official UQ Logo

The shield and the words 'The University of Queensland' and 'Australia' in the supplied configuration and colours comprise the UQ logo. None of these elements should be moved, amended or recoloured. The logo should only be resized in proportion – do not squash or stretch it.
 
The logo must stand alone in a clear area, free of any other material. (Use a measure equal to half the width of the shield in the logo to determine the minimum area that must be left clear around the entire logo.)
 
The University of Queensland logo is not to be used for any purpose other than the title page in this thesis template. The logo is not to be used to advertise, or to imply the University's endorsement of, an external company, product or service.

## Useful R Markdown references

The following references are a useful starting point for learning R Markdown:

* R Markdown by RStudio: https://rmarkdown.rstudio.com/lesson-1.html
* bookdown: Authoring Books and Technical Documents with R Markdown: https://bookdown.org/yihui/bookdown/
* R Markdown: The Definitive Guide: https://bookdown.org/yihui/rmarkdown/
* R Markdown Cheatsheet: https://github.com/rstudio/cheatsheets/raw/master/rmarkdown-2.0.pdf
* R Markdown Quick Reference: https://www.rstudio.com/wp-content/uploads/2015/03/rmarkdown-reference.pdf
