# India Crop Production & Insurance Risk Analysis

An end-to-end data analysis project exploring 20+ years of Indian agricultural production data alongside PMFBY (Pradhan Mantri Fasal Bima Yojana) crop insurance records. Built as part of the M.Sc. Mathematics & Statistics curriculum at IIT Tirupati.

## Datasets

| Dataset | Records | Source |
|---|---|---|
| `APY.csv` | 345k+ rows | Area, Production & Yield by State/District/Season/Crop |
| `PMFBY coverage.csv` | — | Crop insurance coverage by state, season, company |
| `PMFBY statistics.csv` | — | District-level farmer participation, demographics, premiums |
| `in.json` | — | India state-level GeoJSON for choropleth mapping |

## Key Analyses

**Production Analysis (APY dataset)**
- Seasonal analysis — top-producing states per year for Rabi and Kharif seasons
- Drought year detection using aggregate production dip
- State-wise and crop-wise production rankings (Rice, Sugarcane, etc.)
- CAGR computation for long-term production trend assessment
- Crop recommendation by year based on historical production

**Risk & Insurance Analysis (PMFBY datasets)**
- Yield variability using Coefficient of Variation — identifying highest-risk crops for insurance
- GOI vs. state subsidy share breakdown by crop and region
- Farmer participation trend analysis — 2016 to 2023
- District-level area insured and loanee count distribution
- Premium rate computation: Gross Premium / Sum Insured by state

**Geospatial Visualization**
- Choropleth maps of farmer participation and premium rates across Indian states using GeoPandas and a GeoJSON shapefile
- Interactive input-based filtering tool (Year × Season × Crop × Min. Production)

**Exploratory Data Analysis**
- Correlation heatmaps across numerical features
- Outlier detection using IQR fencing
- Pairplots and boxplots by categorical variable
- Categorical cardinality analysis (State, District, Crop, Season)

## Tech Stack

- **Python**: Pandas, NumPy, Matplotlib, Seaborn, GeoPandas
- **Environment**: Jupyter Notebook

## Setup
```bash
git clone https://github.com/mehakjain-hub/india-crop-insurance-risk-analysis.git
cd india-crop-insurance-risk-analysis
pip install -r requirements.txt
jupyter notebook AgricultureProject.ipynb
```

## Requirements
- Pandas
- Numpy
- Matplotlib
- Seaborn
- Geopandas
- Jupyter

## Author
Mehak Jain - M.sc. Mathematics & Statistics, IIT Tirupati (2025-2027)
