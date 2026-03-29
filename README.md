# Life Expectancy Analysis

Data analysis of the factors influencing life expectancy across 193 countries from 2000 to 2015, using the [Life Expectancy (WHO)](https://www.kaggle.com/datasets/kumarajarshi/life-expectancy-who) dataset.

## Analysis

- **Data cleaning:** missing values were imputed using country-grouped interpolation to preserve temporal trends, alongside column normalisation.
- **EDA:** distribution, trend, and correlation analysis broken down by development status, region, and year.
- **Interactive visualisations:** animated choropleth map and scatter plots built with Plotly, plus a correlation heatmap and pairplots.
- **Descriptive statistics:** per-feature distribution profiles covering skewness, mean, median, and standard deviation.
- **PCA:** dimensionality reduction applied to key health and socioeconomic features.
- **Clustering:** K-Means clustering with the elbow method, and Agglomerative Hierarchical Clustering using Ward linkage, compared via silhouette scoring.

## Key Findings

- Developed countries show consistently higher life expectancy than developing nations. This gap narrowed gradually between 2000 and 2015 as health infrastructure improved across lower-income regions.
- Schooling is the strongest positive predictor of life expectancy. Countries averaging more than 14 years of schooling cluster tightly in the 75+ life expectancy range.
- Income composition of resources shows a near-linear relationship with life expectancy, suggesting that broader economic equity matters more than raw GDP alone.
- Adult mortality and HIV/AIDS prevalence are the strongest negative predictors, with sub-Saharan African nations heavily represented at the lower end of the distribution.
- Immunisation coverage for Hepatitis B, Diphtheria, and Polio correlates positively with life expectancy, with the effect most pronounced in developing countries where baseline coverage was lowest.
- Clustering identified three distinct country groupings: high-income developed nations, mid-tier developing countries with improving indicators, and low-income nations with high disease burden. These align closely with WHO regional classifications.
