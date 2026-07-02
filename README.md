
This Read Me file was generated on 2026-07-02 by Charlotte Brault


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

- `data/URSN_trial_info.csv` GPS coordinates of the URSN trial locations.

- `data/dat_FHB_URSN_URNFHB.tsv` Curated phenotypic data for the URSN population and for the URN population for FHB traits.

- `data/all_inputs_URN_URSN_URNFHB.rds` List of formatted inputs.

- `data/genotype_information_URN_URSN_URNFHB.tsv` Table of genomic information for URN and URSN populations, notably their source and first year of testing.


## Analysis scripts

### Inputs

- `analysis/explore_inputs.Rmd` In this script, we load the phenotypic data, explore the experimental design, the phenotypic correlations and the genetic composition of the URN and the URSN populations.

- `analysis/extract_genoVal_URN_URSN_FHB.Rmd` In this script, we load the phenotypic data for the FHB traits and extract the BLUEs (Best Linear Unbiased Estimators) for the genotypes in the URN and URSN populations. The BLUEs are used as inputs for the genetic gain analysis and the QTL analysis.

- `analysis/extract_genoVal_URN.Rmd` In this script, we load the phenotypic data for the agronomic traits and extract the BLUEs for the genotypes in the URN population. The BLUEs are used as inputs for the genetic gain analysis.

#### Genetic gain

- `analysis/URN_URSN_FHB_GGAIN_BLUEs.Rmd`. In this script, we load the BLUEs for the FHB traits and the URSN trial information, we compute the genetic gain for three FHB traits (DIS, VSK and DON) in the URSN population and compare it with the genetic gain in the URN population.

### FHB QTLs

- `analysis/URN_URSN_QTL_frequency.Rmd`. In this script, we load phenotypic data and environmental covariates (ECs), we apply Finlay-Wilkinson regression to predict reaction norm intercept, slope, and phenotypic values based on mean phenotype and ECs. We compare the results with genomic prediction.

- `analysis/explore_FHB_QTL_effect_URN-URSN.Rmd`. In this script, we load the BLUEs from the phenoypic data for all the traits and the FHB QTLs for the URN and URSN populations, we explore the effect of the FHB QTLs on the FHB traits (DIS, VSK and DON) and on three agronomic traits (HT, PH and YLD).

### Other

- `index.Rmd`. This script is the index of the project, it contains the description of the project and the links to the different scripts.

- `about.Rmd`. This script contains the information about the project.

- `license.Rmd`. This script contains the license information.



- **output/figures** folder. This folder contains the figures generated in all scripts.

- The **docs** folder contains the rendered Rmd scripts in html format.

# Software and versions

- R version v4.5.3 and RStudio v2025.09.0+387
