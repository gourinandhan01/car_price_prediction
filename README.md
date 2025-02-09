# **Car Price Prediction Analysis**

## **Table of Contents**
- [Problem Description](#problem-description)
- [Business Goal](#business-goal)
- [Dataset Description](#dataset-description)
- [Project Workflow](#project-workflow)
- [Evaluation Results](#evaluation-results)
- [Findings and Insights](#findings-and-insights)
- [Recommendations](#recommendations)
- [Conclusion](#conclusion)

---

## **Problem Description**
A Chinese automobile company aims to enter the US market by setting up a local manufacturing unit and competing with US and European automakers. The company has partnered with a consulting firm to analyze factors that impact car prices in the American market.

The primary objectives are to:
- Identify variables that significantly influence car prices.
- Evaluate how well these variables explain price variations.

This analysis will help the company tailor their designs and business strategies to the US market and understand pricing dynamics for this new market.

---

## **Business Goal**
The company wants to build a car price prediction model using the available independent variables. The model will:
- Predict car prices based on key variables.
- Enable the management to adjust designs and strategies to achieve desired price levels.
- Provide insights into market dynamics for better decision-making.

---

## **Dataset Description**
The dataset consists of a variety of features related to car specifications and market data collected from the American automobile market.
- **Size:** Comprehensive data representing different types of cars.
- **Variables:** Includes both numerical and categorical features related to design, performance, and market preferences.

---

## **Project Workflow**
The project was structured into the following phases:
1. **Data Preprocessing:**
   - Cleaning the dataset, handling missing values, and encoding categorical variables.
2. **Model Selection and Implementation:**
   - Training five regression models:
     - Linear Regression
     - Decision Tree Regressor
     - Random Forest Regressor
     - Gradient Boosting Regressor
     - Support Vector Regressor
3. **Model Evaluation:**
   - Evaluating models using:
     - **R-squared (R²):** Explains variance in car prices.
     - **Mean Squared Error (MSE):** Measures squared prediction error.
     - **Mean Absolute Error (MAE):** Measures average prediction error.

---

## **Evaluation Results**

| **Model**                | **R-squared** | **MSE**          | **MAE**         |
|--------------------------|---------------|-------------------|-----------------|
| **Linear Regression**    | 0.4737        | 4.15 × 10⁷       | 4177.30         |
| **Decision Tree**         | 0.8559        | 1.14 × 10⁷       | 2200.14         |
| **Random Forest**         | 0.9535        | 3.67 × 10⁶       | 1365.35         |
| **Gradient Boosting**     | 0.9306        | 5.48 × 10⁶       | 1700.99         |
| **Support Vector Regressor** | -0.102       | 8.70 × 10⁷       | 5707.17         |

---

## **Findings and Insights**
1. **Best Model:**
   - **Random Forest Regressor** achieved the highest R-squared (0.9535) and lowest MSE (3.67 × 10⁶) and MAE (1365.35), making it the best model for this task.
2. **Strong Alternative:**
   - **Gradient Boosting Regressor** also performed well, with an R-squared of 0.9306.
3. **Poor Performance:**
   - **Support Vector Regressor (SVR)** showed a negative R-squared (-0.102), making it unsuitable for this dataset.

---

## **Recommendations**
1. Deploy the **Random Forest Regressor** as the primary model for car price predictions.
2. Use the model to analyze the impact of significant variables on pricing and optimize car designs accordingly.
3. Perform hyperparameter tuning to further improve the model’s performance.
4. Consider exploring advanced models like XGBoost or LightGBM for further analysis.

---

## **Conclusion**
This project successfully identifies key factors influencing car prices in the American market and provides a robust predictive model. The insights gained from this analysis will enable the company to strategically design cars and create competitive pricing strategies for their US market entry.
