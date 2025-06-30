🏡 Chicago Housing Prices - Regression Modelling Project

📌 Overview
This project explores a regression-based approach to predict housing prices in Chicago using a dataset of 156 properties. It was completed as part of the MM916: Data Analytics in R course and focuses on selecting optimal predictors, transforming variables, and validating linear regression assumptions to build an accurate predictive model.

🎯 Objective
Develop a linear regression model to predict house prices.

Identify significant predictors affecting house prices.

Examine non-linearities and interaction effects.

Validate and interpret the model statistically and visually.

🗃 Dataset
Source: Real_Estate.csv
Each row represents a Chicago house with the following features:

Variable	Description
Price	Price of house (in 10K USD)
Bedroom	Number of bedrooms
Room	Number of rooms
Space	Size of house (sq ft)
Lot	Width of the lot
Tax	Annual tax (in USD)
Bathroom	Number of bathrooms
Garage	Number of garages
Condition	House condition (1 = Good, 0 = Otherwise)

🧪 Methodology
1. Exploratory Data Analysis
Boxplots to detect outliers.

Correlation heatmaps and scatterplot matrices.

Histograms for distribution shape analysis.

2. Data Transformation
Applied Tukey’s transformation on skewed variables (e.g., Space, Tax, Lot).

Used Q-Q plots and p-values to assess normality improvements.

3. Multicollinearity Check
Calculated VIF (Variance Inflation Factor).

Addressed high collinearity by iterative removal or transformation.

4. Model Building
Stepwise regression using AIC minimization.

Compared two models:

Model 1: Basic predictors

Model 2: Included interaction terms (Condition × Lot, Condition × Bathroom)

Final model selected based on AIC, Adjusted R², F-statistic, and residuals analysis.

5. Model Assumptions
Residual vs. fitted plots

Normality of residuals

Homoscedasticity checks

📈 Final Model Performance
R-squared: 0.7838

Significant predictors: TransformedSpace, TransformedLot, TransformedTax, Garage, and interactions with Condition.

Final model explains over 78% of the variation in house prices.

🛠 Technologies
R and RStudio

Libraries: tidyverse, ggplot2, GGally, car, corrplot, MASS, leaps

📚 Learning Outcomes
Application of regression techniques in real-world data.

Model optimization and interpretation.

Practical understanding of variable transformation and interaction effects.
