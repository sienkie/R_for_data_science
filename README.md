# R for data science

This repository contains materials for **R for data science with tidyverse and ggplot2** seminar, conducted as a part of [#NGSeminars series](https://ngschool.eu/ngseminars) by NGSchool Society. The recording is available [here](https://www.youtube.com/NGSchoolEU).

## Running the tutorial materials

### Local setup

Running materials locally require R and RStudio. Follow steps below to setup your environment:

1. clone *OR* download and unzip this repository

2. open *R_for_data_science.Rmd* in RStudio

3. install required packages (see below)

### Running RStudio on the cloud

If you don't have access to R and RStudio you can run it on cloud for free:

1. create account at https://rstudio.cloud/plans/free and log in

2. in your workspace select *New Project* -> *New Project from Git Repo*

3. copy path to this repository

4. install required packages (see below)

### Package installation
    
```r
required_packages <- c("tidyverse", "ggpubr", "palmerpenguins", "PNWColors", "png")

for (pkg in required_packages) {
  if (pkg %in% rownames(installed.packages()) == FALSE){
    install.packages(pkg)
  }
}
``` 
