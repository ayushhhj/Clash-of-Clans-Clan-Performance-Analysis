# Clash of Clans Clan Performance Analysis

## Introduction

This project analyzes player performance in the popular mobile game **Clash of Clans**, focusing on a comparison between Canadian and American clans. Specifically, we aim to answer the question: \_How does the clan war win proportion and its standard deviation differ between players located in the United States and Canada?

### Dataset

The dataset used in this analysis is sourced from [Kaggle](https://www.kaggle.com/datasets/asaniczka/clash-of-clans-clans-dataset-2023-3-5m-clans), which includes information on over 3.5 million clans. This dataset contains information such as clan location, number of wars won, lost, tied, and clan level.

### Objective

Our goal is to compare the performance of Canadian and American clans in terms of:

- Mean war win proportion
- Standard deviation of war win proportion
- Overall clan activity (total number of wars)

## Methods

This project uses various statistical methods, including:

- **Data cleaning**: The dataset was cleaned by removing clans with less than 100 total wars to exclude inactive clans and focus on meaningful competition.
- **Descriptive statistics**: Key summary statistics such as the number of clans, mean total wars, and war win proportions were calculated for each country.
- **Bootstrapping**: To estimate the 95% confidence intervals for the difference in win proportions.
- **Hypothesis testing**: A null hypothesis was tested to determine if there is a statistically significant difference between the win proportions of Canadian and American clans.

### Libraries Used

- `tidyverse`
- `infer`
- `ggplot2`
- `gridExtra`

## Results

The analysis did not find a statistically significant difference in the mean war win proportion between Canadian and American clans. This conclusion was supported by both the bootstrapping method and an asymptotic t-test. The 95% confidence interval for the difference in means included 0, and the p-values were above the significance threshold.

Key findings:

- The mean win proportion for Canadian clans is approximately 0.639, while for American clans, it is approximately 0.628.
- The observed difference in means is very small (approximately 0.01), and this difference is not statistically significant.

## Visualizations

The project includes visualizations of:

- Sample distributions of total wars for both Canadian and American clans.
- Sample distributions of war win proportions.
- Bootstrap distributions with confidence intervals for the difference in means.
- Null model distributions for hypothesis testing.

## Conclusion

The similarity in performance between Canadian and American clans suggests that cultural and geographical proximity may contribute to comparable player skills. However, further research is recommended to explore clan performance across other countries and games within the eSports industry.

## Further Research

Future directions for this project include:

- Expanding the analysis to other countries or regions to see if geographic and cultural factors influence player performance in the eSports industry.
- Exploring other factors, such as clan type and clan level, and their impact on performance.

## References

- Dataset: [Kaggle - Clash of Clans Clans Dataset](https://www.kaggle.com/datasets/asaniczka/clash-of-clans-clans-dataset-2023-3-5m-clans)
- Parsahkov, P., & Zavertiaeva, M. (2018). _Determinants of Performance in eSports: A Country-Level Analysis_.
- Kashcha, M., Yatsenko, V., & Gyömörei, T. (2022). _Country Performance in e-Sport: Social and Economic Development Determinants_.
