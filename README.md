# Vehicle CO₂ Emissions Analysis
## Project Overview
This project analyzes the relationship between vehicle specifications and CO₂ emissions to help manufacturers meet stricter environmental regulations. Through statistical analysis and data visualization, we identify key factors influencing emissions and provide actionable insights for developing cleaner vehicles.

## Key Findings
### 🔥 Fuel Type Impact
- Ethanol vehicles show highest fuel consumption (city & highway)
- Diesel demonstrates lowest fuel consumption
- Regular gasoline generally produces lower CO₂ emissions
- Kruskal-Wallis Test confirmed statistically significant differences in emissions between fuel types (p < 0.05)

### 🚗 Vehicle Characteristics
- Strong positive correlation between engine size/number of cylinders and CO₂ emissions
- Vehicle size significantly impacts emissions (Kruskal-Wallis p < 0.05):
  - Compact: Lowest emissions
  - Midsize: Moderate emissions
  - Large: Highest emissions

### 🏆 Manufacturer Insights
- Honda maintains lowest average CO₂ emissions among major manufacturers
- Potential for reverse-engineering Honda's emission-reduction strategies

## Technologies Used
```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
from scipy.stats import kruskal
```
## Project Structure
```
CO2_Emissions_project/
├── CO2 Emissions Slides Deck                        # Contains slides deck used for presentation
├── CO2 Emissions_Canada.csv                         # Contains dataset used for analysis
├── Data_Analysis_Notebook_CO2_Emissions_Project/    # Jupyter notebooks with data analysis
├── Machine_Learning_Notebook_CO2_Emissions_Project/ # Jupyter notebooks with machine learning code
└── README.md                                        # This file
```

## Dataset Features
- Engine size (L)
- Number of cylinders
- Fuel type (Regular, Premium, Diesel, Ethanol)
- Fuel consumption (city/highway)
- Vehicle class/size
- CO₂ emissions (g/km)

## Statistical Approach
- Non-parametric tests (Kruskal-Wallis) due to non-normal data distribution
- Correlation analysis for continuous variables
- Comparative visualizations:
  -  Box plots (fuel type vs emissions)
  -  Scatter plots (engine size vs emissions)
  -  Heatmaps (variable correlations)

## Recommendations for Manufacturers
1. Prioritize smaller engines (<2.0L) with 4-cylinder designs
2. Optimize gasoline formulations over ethanol blends
3. Benchmark Honda's technologies for emission reduction
4. Develop compact models to meet stricter regulations

## Future Work
- Machine learning model to predict emissions from specifications
- Time-series analysis of emission trends
- Manufacturer-specific deep dive into Honda's technologies
