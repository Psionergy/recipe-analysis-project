# Sweet Success: Analyzing Recipe Ratings with Data Science

## Recipe Analysis Project
**Author**: Timothy Kam  
**Date**: December 9, 2024  

---

# Introduction

Food is an integral part of daily life, not just for sustenance but also for enjoyment and expression. With the rising prominence of online recipe platforms like Food.com, cooking has evolved from being a necessity to becoming an accessible and creative hobby. The digital age has allowed recipes to be rated, reviewed, and shared by millions, offering invaluable insights into public culinary preferences and trends.

This project aims to leverage data science to analyze and uncover patterns within recipes and user interactions on Food.com. Specifically, the research centers around the question:

**"What factors influence the preparation time of recipes, and how can we use these factors to predict recipe preparation time effectively?"**

Understanding recipe preparation times is essential for everyday users planning their meals and for content creators optimizing their recipes for engagement and usability. By identifying trends and predictive factors, this study can help readers better understand the interplay between recipe characteristics and cooking time, making it a practical application of data science.

---

## The Dataset

This analysis uses two datasets sourced from Food.com, containing a wealth of information about recipes and user interactions:

### `recipes` Dataset
This dataset contains **83,782 rows**, each representing a unique recipe, with the following key columns relevant to this study:

| Column            | Description                                                                                                     |
|-------------------|-----------------------------------------------------------------------------------------------------------------|
| `name`            | Recipe name                                                                                                    |
| `id`              | Unique identifier for each recipe                                                                              |
| `minutes`         | Time (in minutes) to prepare the recipe                                                                        |
| `n_steps`         | Number of steps in the recipe                                                                                  |
| `n_ingredients`   | Number of ingredients required for the recipe                                                                  |
| `tags`            | List of Food.com tags associated with the recipe, such as "quick" or "vegetarian"                              |
| `nutrition`       | Nutrition details including calories, fat, sugar, protein, sodium, and carbohydrates                           |
| `description`     | A user-provided description of the recipe                                                                      |
| `steps`           | Text outlining the recipe steps                                                                               |
| `ingredients`     | Text listing the ingredients for the recipe                                                                    |

### `interactions` Dataset
This dataset contains **731,927 rows**, each capturing a user's interaction with a specific recipe. The key columns are:

| Column      | Description                                   |
|-------------|-----------------------------------------------|
| `user_id`   | Unique identifier for the user               |
| `recipe_id` | Unique identifier linking to a recipe        |
| `date`      | Date when the interaction occurred           |
| `rating`    | Rating given by the user to the recipe (1–5 scale) |
| `review`    | Textual review provided by the user          |

---

## Relevance of the Research Question

The question about predicting recipe preparation times is practical and widely applicable:

1. **For Everyday Users**: Knowing the estimated time to prepare a recipe helps in meal planning, especially for busy individuals or families.  
2. **For Recipe Creators**: Identifying key factors influencing preparation time allows them to optimize recipes to suit specific audiences, like those seeking quick meals or more elaborate dishes.  
3. **For Data Enthusiasts**: This project showcases how exploratory data analysis, feature engineering, and predictive modeling can work together to address a real-world problem.  

---

By addressing this question, the project not only provides actionable insights for recipe users and creators but also highlights the power of data science in uncovering patterns and making predictions in everyday scenarios. This work underscores how leveraging the wealth of data in online platforms like Food.com can improve user experiences and enhance decision-making.
