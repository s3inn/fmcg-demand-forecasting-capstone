\# Data Directory



This directory contains datasets used in the FMCG Global Demand Planning and Forecasting capstone project.



\## Dataset Files



\### fmcg\_sales\_features.csv

Contains the engineered daily demand dataset used for forecasting.



The dataset includes:

\- Daily aggregated units sold by SKU.

\- Lag features (1, 7, 14, 28 and 30 days).

\- Rolling mean features (7, 14, 28 and 30 days).

\- Calendar features including day of week, month and weekend indicators.



\### Datasets excluded from GitHub



The original dataset (`fmcg\_sales\_3years\_1M\_rows.csv`) and cleaned dataset (`fmcg\_sales\_cleaned.csv`) are stored locally and excluded from the repository because of their large file sizes.



\## Reproducibility



The original dataset is required to reproduce the complete analysis. The project notebooks document the data exploration, cleaning, feature engineering and forecasting workflow.

