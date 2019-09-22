BootStrap: docker
From: asachet/rocker-stan

%labels
  Maintainer Marc J Williams

%help
  Singularity image for following paper:

%post
  # add R packages from CRAN
  Rscript -e "install.packages(pkgs = c('devtools', 'cowplot', 'gtools', 'argparse','jcolors', 'ggthemes', 'viridis','Hmisc','ggridges', 'readxl',
  'bayesplot', 'modelr', 'ggforce'), \
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

  # add R packages from github
   Rscript -e "library(devtools); install_github('marcjwilliams1/dndscv')"
