# A Tale of Two Cities: Comparative Public Safety Analysis 🌉

## Project Overview

A comprehensive **comparative data mining analysis** of public safety patterns in San Jose and San Francisco. This project discovers and analyzes the unique "fingerprint" of each Bay Area city's urban dynamics by investigating the **what, when, and where** of public safety events.

## Team Members

- **Rajeev Ranjan Chaurasia** (018283733)
- **Tushar Singh** (018282446)
- **Vatsal Gandhi** (018274841)
- **Jeevan Kurian** (017739397)

## Datasets

### San Francisco
**Source:** [DataSF - SFPD Incident Reports (2018-Present)](https://data.sfgov.org/Public-Safety/Police-Department-Incident-Reports-2018-to-Present/wg3w-h783)

### San Jose
**Source:** [City of San Jose - Police Calls for Service](https://data.sanjoseca.gov/dataset/police-calls-for-service)

## Project Goals

We investigate three analytical dimensions across both cities:

1. **Temporal Analysis** 🕐 (Rajeev)
   - Compare weekly and seasonal patterns
   - Identify temporal similarities and differences

2. **Spatial Analysis** 🗺️ (Tushar - SF, Jeevan - SJ)
   - DBSCAN clustering for hotspot identification
   - Compare dense city (SF) vs. sprawling city (SJ) patterns

3. **Categorical Analysis** 📊 (Vatsal)
   - Association rule mining (Apriori)
   - Cross-city incident type relationship comparison

## Repository Structure

```
sjsf-public-safety-mining/
├── data/
│   ├── raw/                           # Raw data from both cities
│   │   ├── sfpd_incidents.csv        # San Francisco data
│   │   └── sjpd_calls.csv            # San Jose data (to be added)
│   └── processed/                     # Cleaned, harmonized datasets
│       ├── sf_incidents_cleaned.csv   # Preprocessed SF data
│       └── sj_calls_cleaned.csv       # Preprocessed SJ data
├── notebooks/
│   ├── 01_data_preparation.ipynb      # Data cleaning & harmonization
│   ├── 02_sf_eda.ipynb               # San Francisco analysis
│   ├── 03_sj_eda.ipynb               # San Jose analysis (Jeevan)
│   ├── 04_sf_spatial_analysis.ipynb   # SF DBSCAN clustering (Tushar)
│   ├── 05_sj_spatial_analysis.ipynb   # SJ DBSCAN clustering (Jeevan)
│   ├── 06_association_mining.ipynb    # Cross-city categorical analysis (Vatsal)
│   └── 07_comparative_synthesis.ipynb # Final comparative insights
├── src/                               # Reusable Python modules
├── ONBOARDING.md                      # Team setup guide
├── README.md                          # This file
└── requirements.txt                   # Dependencies
```

## Getting Started

Refer to [ONBOARDING.md](ONBOARDING.md) for:
- Environment setup
- Data acquisition instructions
- Team workflow guidelines

---

**Course:** CMPE 255 - Data Mining  
**Institution:** San José State University  
**Last Updated:** October 2025