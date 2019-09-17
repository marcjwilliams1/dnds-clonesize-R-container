BootStrap: docker
From: asachet/rocker-stan

%labels
  Maintainer Marc J Williams

%help
  Singularity image for following paper:

%post
  # add R packages from CRAN
  Rscript -e "install.packages(pkgs = c('devtools', 'cowplot', 'gtools', 'argparse','jcolors', 'ggthemes', 'viridis','Hmisc','ggridges', 'readxl',
  'bayesplot'), \
      repos='https://cran.revolutionanalytics.com/', \
      dependencies=TRUE, \
      clean = TRUE)"
