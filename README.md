## ELM 2024 Analysis

This directory is for the analysis code related to X

## Top-level files

 - .gitignore: Git ignore
 - _quarto.yml: Quarto rendering configuration
 - README.md: this file

## Directory Structure

 - Data/: Contains the raw and/or preprocessed data
 - Figures/: Contains figures in pdf, png, and svg format.
 - Helpers/: Contains helper functions used just for this analysis
 - Models/: Contains already-completed statistical models
 - Writeups/: Contains .qmd files with analysis code and writing

### Data

  - elexicon_metrics.csv: Lexical measures from the elexicon project
  - exp_data.rds: Lexical decision data, preprocessed to omit some participants

### Figures

  - ldonly_basemodel_epred_speedup2: Posterior distribution as percent change for critical conditions
  - predicted_condition_RT: Posterior predicted RTs by-condition (no intonation included/averaged acros intonation conditions)

### Models
  
* denotes the model reported in the text

  - alldata_mdl_notune.rds: Condition-only model with a simpler effect structure
  - alldata_mdl_notune.rds*: Condition-only model with a more complex effect structure
  - base_critical_WKSLP.rds*: Critical trial model
  - base_nosigma_WKSLP.rds: Critical trial model with no sigma parameter

### Writeups

 - elm_writeup.html: Rendered output of elm_writeup.qmd
 - elm_writeup.qmd: Analysis code, which fits the models and produces the figures.