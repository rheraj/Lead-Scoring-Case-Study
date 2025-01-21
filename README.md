# Lead-Scoring-Case-Study

# X Education Analysis  

This project focuses on analyzing customer data for X Education to identify strategies for attracting more industry professionals to enroll in their courses. The dataset provided insights into customer behavior, including site visits, time spent, traffic sources, and conversion rates.

---

## Objectives  

1. Analyze the dataset to understand customer behavior.  
2. Clean and preprocess the data for effective modeling.  
3. Build and evaluate predictive models to identify factors influencing conversions.  
4. Provide actionable recommendations to improve conversion rates.  

---

## Steps Undertaken  

### 1. Data Cleaning  
- Replaced irrelevant entries like "select" with null values.  
- Assigned "not provided" for some null entries to preserve data.  
- Consolidated location data into three categories:  
  - **India**  
  - **Outside India**  
  - **Not Provided**  

### 2. Exploratory Data Analysis (EDA)  
- Removed irrelevant elements in categorical variables.  
- Verified that numeric data was clean and free of significant outliers.  

### 3. Feature Engineering  
- Created dummy variables for categorical data, excluding "not provided."  
- Normalized numeric data using MinMaxScaler.  

### 4. Train-Test Split  
- Split the data into:  
  - **70% training set**  
  - **30% testing set**  

### 5. Model Development  
- Performed Recursive Feature Elimination (RFE) to identify the top 15 features.  
- Removed features with:  
  - Variance Inflation Factor (VIF) > 5  
  - p-value > 0.05  

### 6. Model Evaluation  
- Used a confusion matrix and ROC curve to evaluate performance.  
- Achieved ~80% accuracy, sensitivity, and specificity with an optimal cut-off value of 0.35.  

### 7. Precision-Recall Analysis  
- Found a cut-off of 0.41, yielding:  
  - **Precision:** 73%  
  - **Recall:** 75%  

---

## Key Insights  

The most influential factors driving customer conversions were:  

1. **Behavior Metrics**  
   - Total time spent on the website.  
   - Total number of visits.  

2. **Lead Sources**  
   - Google  
   - Direct traffic  
   - Organic search  
   - Welingak website  

3. **Last Activities**  
   - SMS interactions  
   - Olark chat conversations  

4. **Lead Origin**  
   - Generated via the "Lead Add Format."  

5. **Customer Profile**  
   - Occupation as a working professional.  

---

## Recommendations  

To improve conversion rates, X Education should focus on:  
- Enhancing website engagement to increase time spent and visits.  
- Strengthening marketing efforts on high-performing lead sources (Google, organic search, etc.).  
- Leveraging SMS and chat conversations for effective follow-ups.  
- Targeting working professionals with tailored campaigns.  

By implementing these strategies, X Education can effectively boost enrollments and achieve sustained growth.  

---

## Technologies Used  

- **Python**: Data cleaning, analysis, and modeling.  
- **Pandas**: Data manipulation.  
- **NumPy**: Numerical computations.  
- **Scikit-learn**: Model building and evaluation.  
- **Matplotlib & Seaborn**: Data visualization.  

---

## How to Use  

1. Clone the repository:  
   ```bash
   git clone https://github.com/your-username/x-education-analysis.git
