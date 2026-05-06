# Who Can Still Afford to Live Here?
<sub>Remote Work, Migration, and Housing Dynamics in the Bay Area</sub> 

## Project Background
This project builds on an initial research proposal developed as part of a coursework assignment. The original proposal examined how the rise of remote work reshaped migration patterns and housing affordability, particularly through the "Donut Effect", where higher-income households relocated from urban centers to more affordable surrounding suburban areas.
The proposal introduced a Dynamic Local Income Tax (DLIT) as a potential policy intervention to reduce high-income migration into lower-cost cities and mitigate affordability pressures. While the original work focused on experimental design, this project extends that framework through empirical analysis and a simulation model to evaluate how remote-enabled migration and policy intervention interact in practice. 
By moving beyond the initial proposal, this analysis provides a data-driven examination of housing market dynamics in the Bay Area and explores the potential effectiveness of targeted policy responses. 
The original proposal is included in the 'docs/original_research_proposal.pdf' file for reference. 

## Overview
This project analyzes the effect of the rise of remote work on migration patterns and housing outcomes in the San Francisco Bay Area following the COVID-19 pandemic. While remote work expanded significantly following the pandemic, the empirical analysis finds limited evidence of a strong relationship between remote work adoption and rent growth. To better understand the underlying mechanisms, this project develops a simulation model to examine how migration and policy interventions affect housing market outcomes.  

## Key Questions
1. Does the rise of remote work increase rent prices in suburban cities surrounding San Francisco?
2. How do migration patterns shape local housing markets?
3. Can policy interventions, such as the Dynamic Local Income Tax (DLIT), influence local housing market outcomes?

## Methodology
### 1. Empirical Analysis
- Uses economic, housing, and housing data from ACS & rent price data from Zillow
- Constructs **rent growth acceleration** to measure post-pandemic changes
- Runs regression models to test relationships between rent growth acceleration and:
  - Remote work
  - Income
  - Housing supply
  - Rent dynamics

### 2. Simulation Model
- Simulates household relocation choices
- Households choose cities based on:
  - Rent
  - Amenities
  - Tax costs (DLIT scenario)
- Housing markets respond dynamically to migration flows
  
## Key Findings
- Remote work does **not** show a strong direct relationship with rent growth across cities
- Pre-existing rent trends are the strongest predictor of post-pandemic rent changes
- Migration from San Francisco can generate localized rent pressure in surrounding cities
- The DLIT policy reshapes migration patterns, primarily by redistributing rent pressure to avoid burdening susceptible regions, rather than eliminating it

## Data Sources
- **Zillow Observed Rent Index (ZORI)** -- Rent prices (2015-2025)
- **American Community Survey (ACS) 5-Year Estimates** -- Income, housing, and remote work data

## How to Run
This project is fully reproducible and can be run locally using the included notebook and datasets. 

1. Clone this repo
```bash
git clone https://github.com/jagresti/remote-work-housing-analysis.git
cd remote-work-housing-analysis
```
2. Install required packages
```bash
pip install pandas numpy matplotlib seaborn statsmodels
```
3. Launch the notebook
```bash
jupyter notebook remote_work_housing_analysis.ipynb
```
4. Run the analysis
   - Open the notebook
   - Click Run All Calls
   - All data paths are relative and included in the repository
