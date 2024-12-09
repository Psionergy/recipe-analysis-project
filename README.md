# Sweet Success: Analyzing Recipe Ratings with Data Science

## Recipe Analysis Project
**Author**: Timothy Kam  
**Date**: December 9, 2024  

---

## Introduction
This project examines a dataset of over 83,000 recipes and their corresponding preparation times to answer the question:  
**What factors influence the time required to prepare a recipe?**

Understanding recipe preparation times helps home cooks and professional chefs optimize their meal planning. The dataset includes features such as:
- **`n_ingredients`**: The number of ingredients in a recipe.
- **`n_steps`**: The number of steps in a recipe.
- **`minutes`**: The time it takes to prepare a recipe (target variable).
- **`mean_ingredient_time`**: The average time per ingredient.
- **`ingredients_per_step`**: The number of ingredients per step.

The dataset has **83,782 rows**, and these features provide insight into the complexity of recipes and their preparation times.

---

## Data Cleaning and Exploratory Data Analysis
### Data Cleaning
The following steps were taken to clean the dataset:
1. Removed recipes with missing or zero values for `minutes`, `n_ingredients`, or `n_steps`.
2. Added engineered features:  
   - `log_minutes`: The logarithm of preparation time for skewed distributions.  
   - `mean_ingredient_time`: Preparation time per ingredient.
   - `ingredients_per_step`: Ingredients per step.

Here is the head of the cleaned DataFrame:
```python
   n_ingredients  n_steps  mean_ingredient_time  ingredients_per_step  log_minutes
0              9       10              4.444444              0.900000     3.713572
1             11       12              4.090909              0.916667     3.828641
2              9        6              4.444444              1.500000     3.713572
