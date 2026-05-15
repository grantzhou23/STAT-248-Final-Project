# STAT-248-Final-Project
A repo for the STAT 248 Final Project on the time series analysis of the US unemployment rate.

# Project Overview

This project analyzes monthly U.S. unemployment rates by age group, focusing on differences between youth, prime-age, and older workers. The analysis uses FRED/BLS unemployment series and applies exploratory time-series methods, ACF/PACF analysis, spectral analysis, ARIMA modeling, and lagged regression.

# Data

The data come from FRED/BLS monthly seasonally adjusted unemployment series:

- Overall unemployment rate: `UNRATE_overall`
- Youth unemployment rate, ages 16–24: `UNRATE_youth`
- Prime-age unemployment rate, ages 25–54: `UNRATE_prime`
- Older-worker unemployment rate, ages 55+: `UNRATE_older`

The raw CSV files are stored in the `data/` folder.

# Reproducibility

Install the required packages:

```bash
pip install -r requirements.txt
```

Then open the notebook in the Code/ folder and run it from top to bottom.

# Methods

The notebook includes:

- Data cleaning and merging of monthly unemployment series
- Exploratory data analysis of levels, standardized series, and distributions
- ACF/PACF analysis before and after first differencing
- Spectral analysis using periodograms
- ARIMA modeling and residual diagnostics
- Time-lagged regression of youth unemployment changes on other unemployment series

# Main Findings

Youth unemployment is consistently higher and more volatile than unemployment for prime-age and older workers. However, all age groups share broad cyclical movements, suggesting that common macroeconomic conditions drive much of the variation. The COVID-19 period appears as a major shock throughout the analysis. 

# Repository Structure

```text
.
├── Code/              # Reproducible analysis notebook 
├── Data/              # Raw unemployment data
├── Figures/           # Output plots
├── Report/            # Converted report
├── README.md
├── requirements.txt
└── LICENSE
