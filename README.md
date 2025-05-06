# 🎥 Predicting IMDb Movie Gross Revenue using Multiple Linear Regression

This is a group based project that I made for the course **STA302: Method of Data Analysis 1** at the University of Toronto. The objective was to build a predictive model using **Multiple Linear Regression Method** and understand the key factors influencing a movie’s **Gross Revenue**, a crucial measure of financial success in the film industry. Given the high production costs and the risky nature of movie investments, our analysis aims to offer evidence-based insights for filmmakers and producers. The entire report/project is created by **R** using R studio.

## 🎯 Project Objective
Answer this question:

**To what extent can IMDb rating, Metascore, Release Year, Movie Genre, and Production Cost predict the Gross Revenue of Movies?**

This study / report investigates how **audience reviews**, **critics** **production budgets**, and **genre choices** influence a movie’s box office performance. We aim to identify statistically significant predictors that can help decision-makers allocate resources more effectively and reduce financial risk.

## 📊 Dataset Description

We combined and cleaned two publicly available datasets from **Kaggle**:
- [IMDb Top 2000 Movies Dataset](https://www.kaggle.com/datasets/prishasawhney/imdb-dataset-top-2000-movies): Contains IMDb ratings, release year, genres, and more.
- [The Movies Dataset by Rounak Banik](https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset): Includes production budget and other metadata.

We merged the datasets by matching movie titles to ensure each observation contained all required variables: IMDb rating, Metascore, release year, genre, production budget, and gross revenue. Note that the dataset provided in this repository is the combined one.

## The procedure of this study:
1. **Exploratory Data Analysis (EDA)**:
   - Visualized the distribution of each variable using histograms and pie charts.
   - Identified skewness and potential outliers.
     
2. **Initial Model Building**:
   - Fitted a multiple linear regression model using raw variables.
   - Performed diagnostic checks for linearity, homoscedasticity, normality of residuals, and multicollinearity.
     
3. **Box-Cox Transformation**:
   - Applied transformation to meet regression assumptions.
   - Improved model fit and residual diagnostics.
     
4. **Variable Selection**:
   - Conducted F-tests, t-tests, and Partial F-tests to determine the significance of each predictor.
     
5. **Model Validation**:
   - Detected and analyzed influential points using standardized residuals, leverage values, and Cook's distance.
   - Evaluated model fit using adjusted R-squared and residual plots.
  
## ✅ Final Model Summary

- **Adjusted R-squared**: ~0.396 (indicating moderate explanatory power)
  
- **Significant Predictors**:
  - IMDb Rating (positive correlation)
  - Metascore (positive correlation)
  - Production Budget (strongest positive effect)
  - Release Year (negative correlation)
  - Genre (varied effects based on category)
    
- **Model sastified all assumption** after transformation.
  
- **Outliers and leverage points** were investigated, and influential observations were either retained or automatically excluded by R.

This repository contains the following files:
- **Final Proposal**

- **Final Report**

- **QMD file of the R codes used**

- **Combined Dataset**



