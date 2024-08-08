## ELM 2024 Analysis

This respository presents the analysis code for
*Relating Scalar Inference and Alternative Activation: A View from the Rise-Fall-Rise Tune in American English*
(Sostarics, Ronai, and Cole 2024).

We only include the code related to the specific analyses and figures presented in the paper.

## Top-level files

 - .gitignore: Git ignore
 - _quarto.yml: Quarto rendering configuration
 - ELM2024_Analysis.Rproj: R Project File
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
  - SI_model_data_elm.rds: Preprocessed inference task data

### Figures

  - avg_si_plot: Empirical SI rate averages (Fig. 2 of the paper)
  - pctchange: Posterior percent change distributions (unedited Fig. 4 of the paper)
  - pctchange-fixed: Edited percent change plot with fixed axes (Fig. 4 of the paper)
  - predicted_condition_RT: Posterior predicted RTs by-condition (Fig. 3 of the paper)

### Models

Note that the model files are not on github since they're so large; they are on the osf at https://osf.io/bc6a2/.

* denotes the model reported in the text

  - alldata_mdl_notune.rds: Condition-only model with a simpler effect structure
  - alldata_mdl_notune.rds*: Condition-only model with a more complex effect structure
  - base_critical_WKSLP.rds*: Critical trial model
  - base_nosigma_WKSLP.rds: Critical trial model with no sigma parameter
  - SI_mdl.rds*: Logistic regression model for the inference task results

### Writeups

 - elm_lexdec_analysis.html: Rendered output of elm_lexdec_analysis.qmd
 - elm_lexdec_analysis.qmd: Analysis code for the lexical decision task, which fits the models and produces the figures.
 - elm_si_analysis.html: Rendered output of elm_si_analysis.qmd
 - elm_si_analysis.qmd: Analysis code for the inference task, which fits the models and produces the figures.
