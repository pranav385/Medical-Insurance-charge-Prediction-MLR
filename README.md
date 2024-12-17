# Medical Insurance Charges Prediction

This project aims to predict medical insurance charges using **Multiple Linear Regression**. The goal is to explore how various factors like age, BMI, smoking habits, and others influence insurance charges. The project includes detailed steps of data preprocessing, exploratory data analysis (EDA), model training, and evaluation.

## Project Overview

In this project, I used a real-world dataset to predict the medical insurance charges based on different features like age, BMI, smoking status, and more. I explored multiple approaches, refined features, and tested various techniques to improve the model's performance.

### Key Steps in the Project:

1. **Data Preprocessing**:
   - **Null Values**: Handled missing data to ensure the integrity of the dataset and avoid biased results.
   - **Duplicate Values**: Removed any duplicates from the dataset to avoid repetition and prevent skewing of results.
   - **Outliers**: Detected and managed outliers to maintain the consistency and validity of the data.

2. **Exploratory Data Analysis (EDA)**:
   - Performed a thorough analysis of the dataset to understand relationships, distributions, and potential patterns in the features.
   - Identified smoking status, age, and BMI as significant factors influencing the charges, and discarded less impactful features such as `sex` and `region`.

3. **Modeling**:
   - **Initial Model**: Started with all features available (age, BMI, sex, region, children, smoker) and trained a multiple linear regression model.
   - **Feature Refinement**: Removed less impactful features (`sex`, `region`) to improve model performance.
   - **Log Transformation**: Applied a log transformation on the target variable (charges) to stabilize the variance and improve the model's predictive accuracy.

4. **Model Comparison**:
   - Compared the performance of the **log-transformed model** with the non-log-transformed model, evaluating performance based on metrics like **R-squared**, **Adjusted R-squared**, **F-statistic**, and residual analysis.

### Final Conclusion:

- **Best Model**: The **log-transformed model** outperformed the non-transformed model with slightly better **R-squared (0.758 vs 0.750)**, **Adjusted R-squared (0.757 vs 0.749)**, and higher **F-statistic (724.0 vs 693.4)**, indicating a more statistically significant and accurate model.
  
- **Residual Analysis**: The log-transformed model showed a better percentage difference (28.51%) in residuals compared to the non-log-transformed model (42.10%), reflecting better predictive accuracy.

### Conclusion:

In conclusion, this project demonstrates how feature engineering, data preprocessing, and model transformations (like log transformation) can improve the performance of a regression model. The log-transformed model provides slightly better predictive accuracy, statistical significance, and overall performance. 

### Learnings & Insights:
- Data preprocessing and EDA are crucial for understanding data, refining features, and improving model performance.
- The log transformation technique can stabilize variance and improve predictive accuracy in certain regression models.
- Model evaluation using various metrics such as **R-squared**, **Adjusted R-squared**, and **F-statistic** helps to select the best-performing model.

### Tools & Technologies Used:
- **Python**
- **Pandas**, **NumPy**
- **Matplotlib**, **Seaborn**
- **Scikit-learn** for Regression Modeling
- **Jupyter Notebook**

### Dataset:
The dataset used in this project was obtained from [Kaggle's Medical Insurance dataset](https://www.kaggle.com/datasets), which contains various features like age, BMI, smoking status, and charges.

### Learnings:
This project allowed me to enhance my skills in **data preprocessing**, **EDA**, **multiple linear regression**, and **model evaluation**. I also explored the impact of **log transformation** and **feature engineering** on model performance.

