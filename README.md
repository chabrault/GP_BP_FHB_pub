
This Read Me file was generated on 2026-11-03 by Charlotte Brault


# General information

## Title of Dataset

Supporting data for **Strategic integration of multiple wheat breeding programs and regional nurseries for genomic prediction of Fusarium head blight resistance**.

## Author Information

### Principal Investigator Contact Information

James A. Anderson

Department of Agronomy and Plant Genetics, University of Minnesota 411 Borlaug Hall, 1991 Buford Circle St. Paul, MN 55108

Email: [ander319\@umn.edu](mailto:ander319@umn.edu){.email}

ORCID: 0000-0003-4655-6517

### Associate or Co-investigator Contact Information

Jason D. Fiedler

USDA-ARS Cereal Crops Research Unit Edward T. Schafer Agricultural Research Center, Fargo, ND, USA

Email: [jason.fiedler\@usda.gov](mailto:jason.fiedler@usda.gov){.email}

ORCID: 0000-0001-7736-4484

### Associate or Co-investigator Contact Information

Dr. Charlotte Brault

Department of Agronomy and Plant Genetics, University of Minnesota 411 Borlaug Hall, 1991 Buford Circle St. Paul, MN 55108

Email: [cbrault\@umn.edu](mailto:cbrault@umn.edu){.email} / [charlotte.brault\@live.com](mailto:charlotte.brault@live.com){.email}

ORCID: 0000-0001-7892-4236

-   Date of data collection (single date, range, approximate date): 1995-2024

-   Geographic location of data collection: Northern Great Plains-Midwest of the U.S (MN, ND, SD, MT, Manitoba)

-   Information about funding sources that supported the collection of the data: U.S Wheat and Barley Scab Initiative, USDA-ARS.

-   Overview of the data: 



# Sharing/Access Information

Licenses/restrictions placed on the data: GNU-GPL3

# Data and file description

## Data

- `data/BP_TPE_LOC.csv` GPS coordinates of the URN and URSN trial locations.

- `data/inputs_GP_BP_FHB.rds` List of formatted inputs.


## Analysis scripts

### Inputs

- `analysis/explore_geno-pheno_BP.Rmd` In this script, we load the phenotypic data, explore the experimental design, 
the phenotypic correlations and the genetic composition of the breeding programs and of the URN and the URSN populations.

- `analysis/extract_gen-rel_prediction-scenario.Rmd` In this script, we load the input and determines the training and testing sets for the various prediction scenarios. 
For each prediction fold, we estimate the genetic relatedness between the training and testing sets and we save the results in the tsv file" `output/genom-pred_all-scenarios_genetic-relatedness_Rdist.tsv`. 



### Genomic prediction

- `analysis/genom_pred_btw-BP.Rmd` In this script, we perform genomic prediction of FHB resistance across breeding programs with various prediction scenarios. 
The results are combined and saved in the tsv file `output/genom-pred_all-scenarios_GBLUP-method_BPs_pred-ab.tsv`.


### Analyze results

- `analysis/analyze_genom_pred.Rmd` In this script, we analyze the results of the genomic prediction across breeding programs and we generate the figures and tables for the manuscript. 

- `analysis/analyze_GP_obs_pred.Rmd` In this script, we analyze the results of the genomic prediction across breeding programs and we generate the figures and tables for the manuscript.

- `analysis/pred-ability_response_culling.Rmd`. In this script, we simulate two correlated variables for a range of predictive ability and culling fraction and we estimate the true positive rate.

### Other

- `index.Rmd`. This script is the index of the project, it contains the description of the project and the links to the different scripts.

- `about.Rmd`. This script contains the information about the project.

- `license.Rmd`. This script contains the license information.



- **output/figures** folder. This folder contains the figures generated in all scripts.

- The **docs** folder contains the rendered Rmd scripts in html format.

# Software and versions

- R version v4.6.1 and RStudio v2026.10.1
