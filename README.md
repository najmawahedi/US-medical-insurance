# U.S. Medical Insurance Costs Analysis

This project explores a dataset containing information about U.S. medical insurance costs. The goal is to understand the factors influencing medical insurance charges through various data analysis techniques.

## Project Overview

In this project, we perform the following analyses:

1. **Data Loading and Preparation**: Import the dataset and examine its structure.
2. **Exploratory Data Analysis (EDA)**:
   - Check for missing values and data types.
   - Data visualization of distributions and correlations.
   - Regional analysis of insurance charges.
   - Outlier detection.
3. **Linear Regression Analysis**: Build a linear regression model to identify the most significant predictors of insurance charges.

## Dataset

The dataset contains the following columns:

- `age`: Age of the individual
- `sex`: Gender of the individual (male/female)
- `bmi`: Body Mass Index, a measure of body fat based on height and weight
- `children`: Number of children/dependents covered by the insurance
- `smoker`: Smoking status of the individual (yes/no)
- `region`: Residential area in the U.S. (Northeast, Northwest, Southeast, Southwest)
- `charges`: Medical insurance charges billed by the insurance company

## Key Findings

- **Data Distributions**:
  - The average age is 39, and the average BMI is 30.
  - Approximately 50.5% of individuals are men, and 20% are smokers.
  - The average insurance charge is about $13,270.
  
- **Correlation Analysis**:
  - Smoking status has the highest correlation with medical charges (0.79).
  - Age, BMI, and number of children also positively correlate with charges.

- **Regional Analysis**:
  - The Southeast region shows the highest variability in insurance charges.

- **Outlier Detection**:
  - Significant outliers in the charges variable were identified using the IQR method.

- **Linear Regression**:
  - Smoking status is the most significant predictor of higher charges.
  - Age, BMI, and the number of children also increase charges, though to a lesser extent.
  - Gender has a minimal effect.

## Conclusion

Smoking status significantly impacts medical insurance costs. Age, BMI, and the number of children are also important factors. The Southeast region exhibits higher variability in insurance charges. Our linear regression model explains approximately 78% of the variance in charges, providing valuable insights for consumers, insurers, and policymakers.

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/insurance-cost-analysis.git
   ```
2. Navigate to the project directory:
   ```bash
   cd insurance-cost-analysis
   ```
3. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the notebook:
   ```bash
   jupyter notebook insurance_analysis.ipynb
