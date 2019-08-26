BootStrap: shub
From: granek/singularity-rstudio-tidyverse:3.6.0


  # add R packages from CRAN
  Rscript -e "install.packages(pkgs = c('devtools', 'ggplot2', 'dplyr', 'tidyr', 'stringr', 'cowplot', 'gtools', 'argparse','jcolors', 'ggthemes', 'viridis', 'forcats', 'Hmisc', 'readr', 'ggridges', 'readxl', 'purrr',
   'rstan', 'brms', 'tidybayes', 'bayesplot'), \
      repos='https://cran.revolutionanalytics.com/', \
      dependencies=TRUE, \
      clean = TRUE)"

  #add R packages from bioconductor
   Rscript -e "install.packages('BiocManager')"
   Rscript -e "library(BiocManager); install('GenomicRanges')"
   Rscript -e "library(BiocManager); install('IRanges')"
   Rscript -e "library(BiocManager); install('Biostrings')"
   Rscript -e "library(BiocManager); install('Rsamtools')"
   Rscript -e "library(BiocManager); install('seqinr')"
   Rscript -e "library(BiocManager); install('rtracklayer')"
   Rscript -e "library(BiocManager); install('TCGAbiolinks')"

  # add R packages from github
   Rscript -e "library(devtools); install_github('im3sanger/dndscv')"
