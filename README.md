# classification_of_health_risks_caused_by_fast_food
classification of health risks caused by fast food

# Introduction to Project:
## Background:
Fast food has become a common part of today's diet. With a short time to rest, but no energy deficit, consuming fast food is a common choice to satisfy hunger. 

## Dataset Overview:
This project will analyze 516 menus from seven leading fast food restaurants, reflecting the diversity of choices in the industry. This data analysis aims to understand trends in popularity, nutritional value, and consumer preferences for fast food. 


# Analysis Objective:
- Calculating the average calories, fat, carbohydrates, protein, sodium, sugar, and other nutrients per serving of fast food.
- Comparing the nutritional content of each food menu from various fast food restaurants
- Classify each menu based on macro nutrients and micro nutrients
- Predict the health impact of fast food consumption per menu.
- Make recommendations regarding the consumption of fast food wisely by considering the nutritional content in it.

# Project Timeline:
1. Reading and Understanding datasets (python / excel)
2. Preprocessing Data
3. Exploration Data Analysis
4. Feature Selection
5. Build Model Machine Learning Random Forest Classification & TF-IDF
6. Result of Model 
7. Summary

# EDA:
- Taco Bell has the highest number of menu items (115), followed by Subway (96) and Burger King (70). Chick Fil-A has the fewest menu items (27). In total, there were 515 menu items from all the restaurants analyzed.
- In terms of vitamin categories, most menu items (96.7%) were high in vitamin A, while only a small percentage were high in vitamin C (3.1%) or low in other nutrients (0.19%). This shows that vitamin A was the most common nutrient found in the menus of the seven restaurants.
- For calcium, chicken sandwiches with maple bacon dominate (290mg), followed by cheese curds and various footlong sandwiches (90-100mg), although this calcium content is well within the lower limit of a good nutrient requirement in a single meal of 700 mg.
- High vitamin A was found in premium salads, either with or without chicken (180 mcg RAE), indicating vegetables as the main source. The vitamin a content was still far from the minimum vitamin a requirement of 700 mcg RAE per serving.
- Vitamin C was highest in the avocado turkey bacon sandwich (200 mg), followed by hot pastrami and salad (70-90 mg), showing a variety of vitamin C sources from meat to vegetables. This analysis emphasizes the different sources of nutrients on the menu, with sandwiches and salads being the main contributors.
- The graph shows that the most common health risk was malnutrition (167 cases), followed by renal failure (136 cases) and complications (121 cases).
- While the data does not show a direct correlation between health risks and nutrient content, the average fiber content (4.1) is relatively low compared to total fat (26.6), protein (27.9) and total carbohydrates (45.7).
- This indicates the possibility of nutritional imbalances in the analyzed foods, which may contribute to health risks such as malnutrition and complications.

# Preprocessing Data
1. handling text variables (item) using tf-idf
2. performs label encoding for categorical data: 'restaurant', 'macro_nutrient', 'micro_nutrient', 'health_risk'
3. standardize the data for all numeric data, except the index column
4. combine the results of text handling with tf-idf, label encoding and standardization into a new dataframe called dfm.
   
# Feature Selection:
Selected predictor variable (X): 'sugar', 'sodium', 'micro_nutrient', 'macro_nutrient', 'vector' (tf-idf result) and target variable (y): 'health_risk'

# Build Model Machine Learning
For the classification of health risks caused by nutritional content in fast food, a random forest tree is used because it is resistant to data imbalance. However, this result is likely to change in the future due to periodic experiments and improvements.

# Results Model
Based on the accuracy results of the Random Forest model, it performed very well in classifying health risks, with an overall accuracy of 93.2%. Specifically:
- High Accuracy: The model was able to predict “Malnutrition” and “Diabetes” with perfect accuracy (100%).
- “Kidney Failure” and ‘Complicated’ predictions were also excellent, with precision and recall above 85%.
- Average Performance: Similar macro avg and weighted avg values (93%) indicate that the model has a balanced performance across all health risk classes.
Implications: 
- The model is reliable for identifying health risks based on the trained data.
- It is useful in applications where accurate health risk classification is essential, such as in health data analysis or the development of medical decision support systems.
- The model is particularly good at predicting the “Malnutrition” and “Diabetes” categories.
- It also did very well in predicting the “Kidney Failure” and “Complicated” categories, although not as well as the previous two categories.
Overall, the Random Forest model demonstrated strong classification capabilities and can be a valuable tool in health risk analysis.

# Summary
- This data analysis provides a comprehensive overview of the nutritional profile and potential health risks of fast food menus at several popular restaurants.
- In terms of menu variety, Taco Bell and Subway offer the most choices, while Chick Fil-A has limited options. The majority of the menu items were rich in vitamin A, but relatively low in vitamin C and other nutrients.
- Further nutritional analysis highlighted some important findings:
-   Calcium: While some menu items contained calcium, the amount was below the recommended daily requirement.
-   Vitamins A and C: Premium salads are the main source of vitamin A, while sandwiches and salads provide a variety of vitamin C.
-   Protein and Fiber: Chicken dishes, especially Buttermilk Crispy Chicken Tenders, are rich in protein, exceeding the daily requirement in one serving.
-   Vegetable-based items, such as the Cantina Power Burrito - Veggie, are a good source of fiber.
-   Calories, Fat, Sodium and Sugar: Some items, such as the 20-piece Buttermilk Crispy Chicken Tenders, are very high in calories and fat, far exceeding the recommended limits.
-   Fried chicken and sweet sauce-covered items were consistently high in sodium and sugar.
- These findings indicate potential health risks, such as malnutrition, kidney failure and complications, that may be associated with the nutritional imbalances in these menus. 
- The Random Forest model used to classify health risks showed high accuracy, indicating its potential as a useful tool in health risk analysis.
 
#### Kindly check out details project on my portofolio: https://bit.ly/4lA4Zp6

#### You can find similar dataset in Kaggle: https://www.kaggle.com/datasets/joebeachcapital/fast-food
