# CodTech-Task2
 **Name**: Bharath Chelimalla
 **Company**: CODTECH IT SOLUTIONS
 **ID**: CT12WEUS
 **Domain**: Machine Learning
 **Duration**: December 2024 to March 2025
 **Mentor**: 

### Overview
### Report: Predicting Housing Prices Using Linear Regression  

#### **Objective**  
The primary objective of this project is to develop a predictive model for estimating housing prices based on various features of the Boston Housing dataset. The model is designed to identify key factors influencing housing prices and evaluate their impact using a Linear Regression approach.

#### **Dataset Overview**  
The Boston Housing dataset contains information about houses in Boston, including features like the number of rooms, proximity to the Charles River, and socio-economic indicators. The target variable, `PRICE`, represents the median value of owner-occupied homes.  

Key features used for prediction:  
 **RM**: Average number of rooms per dwelling  
 **CHAS**: Proximity to the Charles River (binary: 0 = far, 1 = close)  
 **AGE**: Proportion of owner-occupied units built before 1940  
 **TAX**: Property-tax rate per $10,000  
 **LSTAT**: Percentage of the lower status of the population  
 
#### **Methodology**  
1. **Data Preparation**  
    **Dataset Loading**: The dataset was fetched from OpenML using the `fetch_openml` function.  
    **Feature Selection**: Five significant features were selected for model development.  
    **Feature Scaling**: Applied `StandardScaler` to normalize features for consistent scaling, improving model performance.
![Screenshot 2024-12-30 175320](https://github.com/user-attachments/assets/a9d4cd72-87f3-4470-bfc3-3e9cd9d4508d)


2. **Model Development**  
    **Data Splitting**: The dataset was split into training (80%) and testing (20%) sets to ensure evaluation on unseen data.  
    **Model Training**: A Linear Regression model was trained on the scaled training data.

![Screenshot 2024-12-30 175303](https://github.com/user-attachments/assets/5acfe54c-4272-4b2d-9295-3609910b9d58)


3. **Evaluation Metrics**  
    **Mean Squared Error (MSE)**: Measures the average squared difference between actual and predicted prices.  
    **R² Score**: Indicates the proportion of variance in the target variable explained by the model.  
    **Model Accuracy**: Represents the percentage of variance correctly predicted by the model on the test set.  

4. **Visualizations**  
    Scatter plot comparing actual vs. predicted prices.
   ![Screenshot 2024-12-30 171528](https://github.com/user-attachments/assets/38d1b58c-73a9-4c57-9054-238e6965b30a)

    Bar chart showcasing the feature coefficients (importance).
    
#### **Results**  
 **Model Performance**  
   ![Screenshot 2024-12-30 175247](https://github.com/user-attachments/assets/66de276b-8156-4349-bf67-0eb22367bfbd)

 **Feature Coefficients**  
  Feature importance based on Linear Regression coefficients:  
   **RM**: Positive coefficient, indicating an increase in rooms leads to higher prices.  
   **LSTAT**: Negative coefficient, showing that higher lower-status population percentages reduce housing prices.  
   **Other features**: Contributed to varying degrees.

#### **Insights**  
1. **Key Influencing Factors**  
    The number of rooms (`RM`) is a significant positive contributor to housing prices.  
    Socio-economic factors (`LSTAT`) have a strong negative impact on prices.  

2. **Model Accuracy**  
    The Linear Regression model performs well in predicting housing prices, as indicated by the R² score and accuracy.  

3. **Visual Validation**  
    The scatter plot demonstrates a good correlation between actual and predicted prices, with most points aligning closely with the diagonal line.  

#### **Conclusion**  
This project successfully develops and evaluates a Linear Regression model to predict housing prices based on selected features. The results show that the model captures the relationship between housing prices and socio-economic as well as structural factors.  
