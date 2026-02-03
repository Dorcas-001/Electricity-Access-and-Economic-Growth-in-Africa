# Electricity Access and Economic Growth in Africa

## Project Overview

This project analyzes the relationship between electricity access and economic growth in selected West and Central African countries, with a specific focus on **Cameroon as the baseline country**. Using panel data from 1990 to 2023, the study examines whether higher electricity access is associated with higher GDP per capita and how robust this relationship remains under increasingly rigorous econometric specifications.




## Research Question

**How is access to electricity associated with economic growth (GDP per capita) in selected African countries, and how robust is this relationship after controlling for country-specific and time-specific factors?**



## Data Sources

All data are publicly available and obtained from reputable international institutions:

- **World Bank – World Development Indicators (WDI)**
  - GDP per capita (constant prices)
  - Electricity access (% of population)

- **International Energy Agency (IEA)**
  - Used for contextual background on electricity access and energy policy

### Countries Included
- Cameroon (baseline)
- Côte d’Ivoire
- Ghana
- Nigeria

### Time Period
- 1990–2023 (annual data)

### Sample Size
- 128 country–year observations



## Variables

### Dependent Variables
- `gdp_pc`: GDP per capita
- `log_gdp_pc`: Natural logarithm of GDP per capita (final model)

### Independent Variable
- `elec_access`: Electricity access (% of population)

### Controls
- Country fixed effects
- Year fixed effects



## Methodology

The empirical analysis follows a stepwise modeling approach:

1. **Descriptive statistics and correlation analysis**
   - Examines basic distributions and associations.

2. **Simple OLS regression**
   - Estimates the unconditional relationship between electricity access and GDP per capita.

3. **OLS with country fixed effects**
   - Controls for time-invariant country characteristics.

4. **OLS with country and year fixed effects**
   - Accounts for common macroeconomic and regional time shocks.

5. **Clustered standard errors (by country)**
   - Corrects for serial correlation and heteroskedasticity in panel data.

6. **Log-transformed GDP per capita (final specification)**
   - Enables percentage-based interpretation and reduces sensitivity to outliers.



## Key Results

- The correlation coefficient between electricity access and GDP per capita is **positive and strong (ρ ≈ 0.67)**.
- In the final log-linear model:
  - A **1 percentage point increase in electricity access** is associated with an **approximately 2.8% increase in GDP per capita**.
- Country fixed effects (baseline: Cameroon):
  - **Ghana:** ≈ 44% lower GDP per capita (statistically significant)
  - **Nigeria:** ≈ 28.6% higher GDP per capita (statistically significant)
  - **Côte d’Ivoire:** No statistically significant difference


## Visual Outputs

The project includes the following figures:

1. Scatter plot of electricity access vs. log GDP per capita  
2. Time trends of electricity access and GDP per capita by country  
3. Histogram of regression residuals  

All figures are labeled, captioned, and referenced in the report.


## Interpretation and Limitations

The results indicate a robust conditional association between electricity access and economic growth. 

## Policy Relevance

Despite these limitations, the consistency and magnitude of the estimated relationship support policy strategies that prioritize:

- Expansion of electricity access
- Improvements in power reliability
- Integration of energy investments with broader economic development reforms


## Repository Structure
- `data/` – inflation datasets  
- `notebooks/` – analysis and modeling notebooks  
- `scripts/` – reusable ARIMA functions  
- `results/figures/` – plots and diagnostics  
- `results/tables/` – comparison tables  

## Author
Ngeyen Dorcas
