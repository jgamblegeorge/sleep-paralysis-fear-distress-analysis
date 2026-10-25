# Predictors of Fear and Distress During Isolated Sleep Paralysis

This repository contains the analysis notebook used for the study **“Predictors of fear and distress during isolated sleep paralysis: an exploratory study.”**

## Study overview

The study examined cognitive and experiential factors related to fear and distress during isolated sleep paralysis (ISP), including dream awareness, dream control, dream skepticism, explanatory beliefs, prior knowledge and experience with sleep paralysis, recognition of ISP, confidence that the perceived threat was not real, and overall outlook toward sleep paralysis.

Analyses included descriptive statistics, Spearman rank correlations, ordinal logistic regression for the primary ordinal outcomes, binary logistic regression for secondary outcomes, Random Forest models with cross-validation, permutation feature importance, and SHAP-based model interpretation.

## Repository contents

- `analysis/Myna_Sleep_Paralysis_Analysis.ipynb` — cleaned analysis notebook used for the manuscript. Saved cell outputs and execution metadata were removed before public release to avoid exposing participant-level survey responses.
- `requirements.txt` — Python packages required to reproduce the analyses.
- `CITATION.cff` — citation metadata for this repository.
- `.gitignore` — prevents raw survey data and generated output files from being committed accidentally.

## Data availability

The participant-level survey dataset is **not included in this repository** to protect participant privacy. The notebook documents the analytic workflow.

## Reproducibility

The notebook was developed and run in Google Colab using Python. To reproduce the analysis, open the notebook in Colab or a compatible Jupyter environment, install the packages in `requirements.txt`, provide the de-identified survey dataset in the expected format, and run the notebook from top to bottom.

The analytic sample excludes respondents who did not report a history of sleep paralysis, respondents younger than 18 years, and respondents reporting a professional diagnosis of narcolepsy. Analyses with missing or non-classifiable responses may use smaller complete-case samples.

Machine-learning analyses were exploratory. Random Forest performance was evaluated using cross-validation, and SHAP values were used to interpret contributions to model predictions. Neither feature importance nor SHAP values should be interpreted as causal effects.

## Authors

- Manaswini Ramanathan — student researcher
- Joyonna Gamble-George — senior mentor

## Citation

Please cite the associated manuscript and this repository if you use the analysis code. See `CITATION.cff` for repository citation metadata.

## Data privacy

Do not commit participant-level survey exports or generated files containing participant responses to this repository.
