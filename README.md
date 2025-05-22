#  Predicting Student Performance using Linear Regression

This project demonstrates the use of **Linear Regression**, a fundamental machine learning algorithm, to predict students' academic performance based on various factors such as hours studied, sleep, and extracurricular activities. Completed during the **DS & ML Bootcamp by Ai DataYard**, the project applies **Simple and Multiple Linear Regression** techniques on real-world data.

---

##  Objective

* To apply Linear Regression for predicting students' performance based on features like:

  * Hours Studied
  * Previous Scores
  * Sleep Hours
  * Sample Question Papers Practiced
  * Extracurricular Activities
* To understand and implement both **Simple Linear Regression** and **Multiple Linear Regression**.
* To train, evaluate, and interpret a regression model using Python.
* To explore how different variables influence student success.



##  Dataset Overview

* **Source**: [Student Performance - Multiple Linear Regression (Kaggle)](https://www.kaggle.com/datasets/nikhil7280/student-performance-multiple-linear-regression)
* **Features**:

  * `Hours Studied`
  * `Previous Scores`
  * `Extracurricular Activities` (Yes/No)
  * `Sleep Hours`
  * `Sample Question Papers Practiced`
  * `Performance Index` (Target Variable)

---

##  Tools & Libraries Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* scikit-learn (LinearRegression, train\_test\_split, LabelEncoder, metrics)



##  Step-by-Step Process

### 1. **Data Loading and Exploration**

* Loaded the dataset using Pandas.
* Displayed the first few rows to understand the structure.
* Checked column data types and dataset dimensions.
* Verified absence of null or duplicate values.

### 2. **Data Preprocessing**

* Used `LabelEncoder` to convert the categorical feature `Extracurricular Activities` to numeric:

  * `Yes` → `1`, `No` → `0`
* Separated the features (`X`) and target variable (`y = Performance Index`).

### 3. **Train-Test Split**

* Split data into training and testing sets (80% train, 20% test).
* Used `random_state=42` for reproducibility.

### 4. **Model Training**

* Created a `LinearRegression` model using `sklearn.linear_model`.
* Trained the model on training data using `.fit(X_train, y_train)`.

### 5. **Model Evaluation**

* Calculated R-squared (coefficient of determination) to evaluate how well the model explains the variance.
* Compared real vs predicted values.
* Visualized predictions using a **scatter plot**.
* Calculated:

  * **Mean Absolute Error (MAE)** – to understand average error.
  * **Model coefficients** – to see the effect of each independent variable.
  * **Intercept** – the baseline prediction when all inputs are zero.



##  Visualizations

* **Scatter Plot** of Real vs Predicted Performance.
* Plots showcasing data distribution and relationships among features.



##  Key Takeaways

* **Linear Regression** is effective for predicting continuous outcomes like performance scores.
* Factors such as **hours studied** and **sample question papers practiced** significantly influence performance.
* **Extracurricular Activities** and **Sleep Hours** also have a measurable impact.
* Model evaluation metrics like **R²** and **MAE** help assess prediction accuracy.
* Understanding coefficients helps in interpreting which features are most impactful.


##  Author

**Maira Nawaz**

[LinkedIn](https://www.linkedin.com/in/mairanawaz/) | [Kaggle](https://www.kaggle.com/mairanawaz) | [Github](https://github.com/Maira-Nawaz)
