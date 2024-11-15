# 🩺 Stroke Prediction and Analysis

This project focuses on analyzing a healthcare dataset to uncover key insights related to stroke risk factors. The analysis aims to assist healthcare providers and insurance companies in understanding the patterns and risk factors associated with stroke, ultimately contributing to better preventive measures and targeted interventions.

## 📊 Dataset Overview

The dataset used in this analysis was obtained from Kaggle. It includes various demographic, medical, and lifestyle features of patients, such as:

- **Gender**
- **Age**
- **Hypertension**
- **Heart Disease**
- **Marital Status**
- **Work Type**
- **Residence Type**
- **Average Glucose Level**
- **BMI**
- **Smoking Status**
- **Stroke (Target Variable)**

The goal is to identify significant risk factors and provide recommendations based on the findings.

## 🛠️ Data Cleaning

1. Removed irrelevant columns (e.g., `id`).
2. Handled missing values in the `bmi` column by filling them with the mean.
3. Converted the `age` column to integer type for consistency.

## 🔍 Key Analyses and Findings

### 1. Age Group Distribution
- The largest group of patients in the dataset is adults (ages 18-60).

### 2. Hypertension and Heart Disease by Gender
- Males show a higher prevalence of heart disease compared to females.
- Hypertension rates are similar across genders.

### 3. Stroke Incidence by Gender
- Stroke incidence is slightly higher among males (5.1%) compared to females (4.7%).

### 4. Impact of Marital Status on Stroke Incidence
- Married individuals have a higher stroke rate compared to unmarried individuals.
- After marriage, males are more likely to experience strokes than females.

### 5. Urban vs. Rural Differences in Glucose Levels and BMI
- No significant difference in stroke incidence between urban and rural residents.
- Average glucose levels are within the normal range, but average BMI indicates overweight status.

### 6. Impact of BMI on Stroke Incidence
- Higher BMI is associated with an increased likelihood of stroke.
- The overweight group shows a significantly higher stroke rate (5.88%).

### 7. Effect of Smoking Status on Stroke Incidence
- Both current and former smokers have higher stroke rates compared to non-smokers.
- The highest stroke rate is observed among former smokers.

### 8. Correlation Analysis
- Age, average glucose level, and BMI all show statistically significant correlations, indicating that these factors are interrelated and may collectively impact stroke risk.

### 9. Influence of Work Type on Stroke Incidence
- Self-employed individuals have the highest stroke rate, possibly due to lifestyle stressors.
- Children and individuals who have never worked have the lowest stroke rates.

### 10. Impact of Medical History on Stroke Incidence
- Patients with a history of hypertension, heart disease, or both are significantly more likely to experience a stroke.
- The highest stroke rate is observed in patients with both hypertension and heart disease.

## 📈 Statistical Hypothesis Testing

The following hypothesis tests were conducted to validate the findings:

1. **Age and Stroke Incidence**: Age significantly affects stroke incidence (Logistic Regression, p < 0.05).
2. **Residence Type and Stroke Incidence**: No significant difference in stroke rates between urban and rural residents (Chi-square test, p > 0.05).
3. **Medical History and Stroke**: Significant relationship between hypertension, heart disease, and stroke (Chi-square test, p < 0.05).
4. **Correlation Among Age, Glucose Level, and BMI**: Significant monotonic relationships (Spearman’s Rank Correlation).
5. **Work Type and Stroke Incidence**: Significant effect of work type on stroke incidence (Chi-square test, p < 0.05).
6. **Smoking Status and Stroke Incidence**: Significant relationship between smoking status and stroke (Chi-square test, p < 0.05).

## 📌 Recommendations

Based on the analysis, the following recommendations are proposed:

1. **Smoking Cessation Programs**: Targeted education and support programs to reduce smoking-related stroke risks.
2. **Early Detection of Hypertension and Heart Disease**: Regular screenings and treatment adherence should be incentivized by insurance companies.
3. **Weight Management**: Implement weight management programs to lower obesity rates and related stroke risks.
4. **Health Interventions for Self-Employed Individuals**: Provide stress management workshops and routine health check-ups for self-employed workers.
5. **Education for Married Individuals**: Promote risk reduction strategies through health education programs tailored for married couples.
6. **Equal Access to Healthcare**: Ensure that health interventions are accessible to both urban and rural populations.
7. **Targeted Interventions for Older Adults**: Develop lifestyle modification programs focused on reducing stroke risks among older adults.

## 📂 Files in This Repository

- **`Stroke_Analysis.ipynb`**: Jupyter Notebook with the full analysis and visualizations.
- **`healthcare-dataset-stroke-data.csv`**: Original dataset (to be added via link).
- **`README.md`**: This file.

## 📊 Summary of Hypothesis Testing Results

| Hypothesis Test                           | Result                                          |
| ----------------------------------------- | ----------------------------------------------- |
| Age affects stroke incidence              | **Reject null hypothesis**                      |
| Residence type affects stroke incidence   | **Fail to reject null hypothesis**              |
| Medical history affects stroke incidence  | **Reject null hypothesis**                      |
| Correlation among age, glucose, and BMI   | **Significant monotonic relationships**         |
| Work type affects stroke incidence        | **Reject null hypothesis**                      |
| Smoking status affects stroke incidence   | **Reject null hypothesis**                      |

## 📬 Contact

If you have any questions or suggestions, please feel free to reach out.

## 📂 Dataset

You can download the dataset from the following link:

**[Dataset Link]([https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset])**

