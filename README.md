#An Investigation into Energy Consumption and Population Growth in Select Countries
#Overview
This repository contains the code, data, and analysis for a project investigating the relationship between energy consumption and population growth in four select regions: India, the United States, the European Union, and Canada. The analysis spans 34 years of data sourced from the World Bank. Using clustering techniques (K-Means) and curve-fitting models, we identify patterns, trends, and future projections for energy use per capita.

#Key goals:

Cluster countries based on energy use and population metrics.
Model historical trends with simple curve fits.
Predict future energy consumption growth.

The project reveals distinct clusters, with the European Union showing the highest average energy use and India the lowest. All regions exhibit growth in energy use, led by India.

#Key Findings

Clustering Results: K-Means identifies 2-3 clusters based on energy-population correlations. EU leads in per-capita energy; India shows rapid growth.
Trends: Energy use rose across all regions (1985-2019 data), with India's growth rate ~3x higher than Canada's.
Predictions: Models forecast continued increases, emphasizing the need for sustainable policies in high-growth areas like India.
Correlations: Strong positive link between population size and total energy use (r > 0.8 in heatmap).

#Data Sources

Primary: World Bank Open Data (1985-2019).
Energy Use: EG.USE.PCAP.KG.OE
Population: SP.POP.TOTL

Regions: India (IN), United States (US), European Union (EU aggregate), Canada (CA).

#Methods

Preprocessing: Normalize features (Min-Max scaling) for clustering.
Clustering: K-Means (k=3) via scikit-learn; Elbow method for optimal k.
Curve Fitting: Polynomial regression (degree 1-3) using scipy; extrapolated to 2030-2050.
Evaluation: Silhouette score for clusters; R² for model fits.

#Limitations and Future Work

Data aggregated at regional level; finer granularity (e.g., per-state) could enhance insights.
Models are simple—future extensions: ARIMA time-series or machine learning (e.g., Random Forest).
Incorporate external factors like GDP or renewable energy adoption.
