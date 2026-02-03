# Modeling Inflation Dynamics and Forecasting in Selected African Economies


## Project Overview
This project studies inflation dynamics and short-term inflation forecasting in selected African economies, with **Cameroon as the baseline country**. Using annual inflation time-series data and ARIMA models, the analysis examines inflation persistence, volatility, and medium-term forecasts, and compares Cameroon’s inflation behavior with Ghana, Nigeria, and Côte d’Ivoire.


## Research Question
How do inflation dynamics differ across selected African economies, and what do short-term forecasts reveal about Cameroon’s inflation trajectory relative to its peers?

## Data Sources
- World Bank – World Development Indicators (WDI)
  - Annual inflation rate (%)

### Countries
- Cameroon (baseline)
- Ghana
- Nigeria
- Côte d’Ivoire

### Frequency
- Annual data (country-specific coverage)

## Variables
- `inflation`: Annual inflation rate (%)
- Lagged inflation terms (AR components)
- Lagged forecast errors (MA components)

## Methodology
1. Data cleaning and restructuring into country-level time series  
2. Visualization of historical inflation trends  
3. Stationarity testing using the Augmented Dickey–Fuller (ADF) test  
4. ARIMA model selection using AIC  
5. Residual diagnostics and model validation  
6. Five-year-ahead inflation forecasting  

## Key Findings
- Cameroon’s inflation is stationary and well modeled by ARIMA(1,0,0), indicating moderate persistence.
- Ghana’s inflation is non-stationary and more volatile, requiring differencing and a higher-order ARIMA model.
- Nigeria shows persistent inflation dynamics with significant AR and MA components.
- Côte d’Ivoire exhibits relatively stable inflation behavior.
- Inflation forecasts differ substantially across countries, highlighting strong country-specific dynamics.

## Policy Relevance
- Supports inflation monitoring using statistical forecasts  
- Highlights the need for country-specific macroeconomic policies  
- Provides benchmarking insights for Cameroon relative to regional peers  

## Repository Structure
- `data/` – inflation datasets  
- `notebooks/` – analysis and modeling notebooks  
- `scripts/` – reusable ARIMA functions  
- `results/figures/` – plots and diagnostics  
- `results/tables/` – comparison tables  

## Author
Ngeyen Dorcas
