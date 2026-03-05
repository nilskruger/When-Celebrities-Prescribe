# When-Celebrities-Prescribe-Drug-Promotion-and-Regulation-on-the-Internet
This repository contains illustrative R code related to a Perspective article.

# About the Code
The R script provided in this repository reproduces the quantitative analysis and figure featured in the article.

## Methodology
* Data Extraction: We use the gtrendshealth R package to pull daily Google Search query fractions for related terms.
* ARIMA Modeling: We use Auto-Regressive Integrated Moving Average (ARIMA) models, trained on pre-event data, to forecast a counterfactual scenario.
* Impact Assessment: We quantify the absolute difference between the observed search volumes and the predicted counterfactual (with 95% confidence intervals) to evaluate the magnitude of the impact.
* Visualization: The code generates the final interrupted time-series visualizations.


## Requirements
```markdown
To run this code, you will need:
* R and RStudio
* A Google Trends for Health API key (to query via the `gtrendshealth` package).
  Reference: https://github.com/CDCgov/gtrendshealth
* The following R packages:
`gtrendshealth`, `forecast`, `ggplot2`, `ggsci`, `systemfonts`, `showtext`, `dplyr`, `patchwork`, `grid`.
```

## Instructions
```markdown
1. Download the `.Rmd` file.
2. Open the file in RStudio.
3. Replace `"YOUR_API_KEY_HERE"` in the Setup chunk with your API key.
4. Run all chunks to reproduce the data downloads, ARIMA forecasts, and plots. 
```
