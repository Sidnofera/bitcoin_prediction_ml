# Predicting Stock Profitability Using Machine Learning

This project applies machine learning techniques to predict whether a particular trade will be profitable or not, based on historical Bitcoin price data. By analyzing patterns and using advanced ML models, the project aims to provide insights into stock market trends.

---

## **Overview**

Machine learning has proven immensely helpful in automating tasks across industries. One such application is predicting whether buying a particular stock will be beneficial. Using Python's robust libraries and machine learning algorithms, this project predicts trading signals based on historical data.

---

## **Dataset**

- **Source:** Bitcoin price data (OHLC) from 17th July 2014 to 29th December 2022.
- **Features:** 
  - Open
  - High
  - Low
  - Close
  - Adj Close (removed as redundant)
  - Additional features engineered: `open-close`, `low-high`, and `is_quarter_end`.
- **Target Variable:** Indicates whether the stock price will increase the next day.

---

## **Modules Used**

- **Pandas:** For data manipulation and analysis.
- **NumPy:** For efficient numerical operations.
- **Matplotlib & Seaborn:** For data visualization.
- **Scikit-learn:** For data preprocessing and model development.
- **XGBoost:** For advanced gradient boosting machine learning.

---

## **Steps Involved**

1. **Data Loading and Preprocessing**
   - Imported OHLC data and performed feature engineering.
   - Added derived features like `open-close`, `low-high`, and `is_quarter_end`.
   - Removed redundant columns and handled missing values.

2. **Exploratory Data Analysis (EDA)**
   - Visualized trends and patterns using line plots, box plots, and distribution plots.
   - Checked correlations among features to avoid redundancy.

3. **Feature Engineering**
   - Extracted `day`, `month`, and `year` from the `Date` column.
   - Created a binary target feature indicating the next day’s price movement.

4. **Model Development**
   - Models used: 
     - Logistic Regression
     - Support Vector Machine (SVM)
     - XGBoost Classifier
   - Data split: 90% training and 10% validation.
   - Evaluated using ROC-AUC score and confusion matrix.

5. **Evaluation**
   - XGBoost showed the highest training accuracy but suffered from overfitting.
   - Logistic Regression provided balanced performance with no overfitting.

---

## **Results**

- **Best Model:** Logistic Regression (balanced performance without overfitting).
- **Challenges:**
  - Insufficient data volume.
  - The complexity of stock market prediction with simple models.

---







