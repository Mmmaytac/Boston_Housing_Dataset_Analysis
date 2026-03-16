# Boston Housing Dataset Analysis

This project performs a statistical analysis of the **Boston Housing Dataset**. The analysis focuses on understanding how different factors affect the **median value of owner-occupied homes (MEDV)**.

## Dataset

The dataset contains information about housing values in suburbs of Boston, including variables such as:

- `MEDV`: Median value of owner-occupied homes
- `CHAS`: Charles River dummy variable (1 if bounded by the river, 0 otherwise)
- `AGE`: Proportion of owner-occupied units built before 1940
- `NOX`: Nitric Oxide concentration
- `INDUS`: Proportion of non-retail business acres per town
- `DIS`: Weighted distances to five Boston employment centres

## Analysis Performed

1. **Correlation Analysis**
   - Examined relationships between continuous variables such as `NOX` and `INDUS`.

2. **Group Comparison Tests**
   - **Levene's Test**: Checked for equality of variances of `MEDV` by `CHAS`.
   - **T-test**: Compared `MEDV` between homes bounded and not bounded by the Charles River.
   - **ANOVA**: Compared `MEDV` among three age groups (`AGE_group`).

3. **Regression Analysis**
   - Fitted a **simple linear regression** model to assess the impact of `DIS` on `MEDV`.

4. **Visualizations**
   - Boxplots for `MEDV` overall and by groups
   - Bar plot for `CHAS`
   - Scatter plots and correlation heatmaps

## Key Insights

- Homes bounded by the Charles River have **significantly different median values** compared to those not bounded.
- The age of homes strongly affects median home values, with older homes showing different pricing patterns.
- There is a **strong positive correlation** between `NOX` and `INDUS`, indicating industrial areas contribute to higher pollution.
- Distance from employment centres (`DIS`) has a **statistically significant positive effect** on median home value, but explains only a small portion of the variation.

## Tools Used

- Python (`pandas`, `numpy`, `seaborn`, `matplotlib`, `scipy`, `statsmodels`)
- Jupyter Notebook for analysis and visualization
