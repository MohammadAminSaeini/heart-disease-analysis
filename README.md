# Heart Disease Analysis

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue.svg?logo=linkedin)](https://www.linkedin.com/in/mohammad-amin-saeini)
[![Kaggle](https://img.shields.io/badge/Kaggle-Profile-blue.svg?logo=kaggle)](https://www.kaggle.com/mohammad-amin-saeini)

## Overview
Understanding the driving factors behind cardiovascular issues is critical for early diagnosis and preventative care. This project explores a medical dataset containing patient records to analyze the features most strongly associated with heart disease. Through data cleaning, descriptive statistics, and targeted visualization, the objective is to uncover the distribution of these clinical features and evaluate their predictive relationship with the target variable (the presence or absence of heart disease).

## Dataset Features
The dataset (`src/heart.csv`) contains 303 patient records across 14 clinical features:
* `age`: Age of the patient in years.
* `sex`: Gender of the patient (1 = male, 0 = female).
* `cp`: Chest pain type (4 values).
* `trestbps`: Resting blood pressure (in mm Hg).
* `chol`: Serum cholesterol in mg/dl.
* `fbs`: Fasting blood sugar > 120 mg/dl (1 = true, 0 = false).
* `restecg`: Resting electrocardiographic results.
* `thalach`: Maximum heart rate achieved.
* `exang`: Exercise-induced angina (1 = yes, 0 = no).
* `oldpeak`: ST depression induced by exercise relative to rest.
* `slope`: The slope of the peak exercise ST segment.
* `ca`: Number of major vessels (0-3) colored by fluoroscopy.
* `thal`: Thalassemia score.
* `target`: Presence of heart disease (1 = disease, 0 = no disease).

## Project Workflow
1.  **Data Inspection & Cleaning**:
    * Evaluated the dataset for missing values and structural inconsistencies. 
    * The dataset was exceptionally clean with 0 missing values. One duplicated row was identified and subsequently dropped, resulting in a finalized dataset of 302 unique records.
2.  **Correlation Analysis**:
    * Computed a Pearson correlation matrix for all numerical features to identify positive, negative, and neutral linear relationships.
    * Visualized these correlations using heatmaps to highlight variables that strongly influence the `target` classification.
3.  **Feature Visualization**:
    * Plotted continuous variable relationships, specifically visualizing Age vs. Serum Cholesterol and max heart rate distributions to spot clustering between patients with and without the disease.
4.  **Conclusion**:
    * The data distribution revealed an interesting anomaly: a lack of positive heart disease cases in expected "danger zones" (such as very high cholesterol or high resting blood pressure ranges), suggesting potential dataset errors or inconsistencies.
    * Assuming the data is structurally accurate, **Exercise Induced Angina (`exang`)** proved to be a highly significant diagnostic factor, exhibiting a remarkably strong correlation compared to other standard medical features.

## Technologies & Libraries Used
* **Python 3**
* **Pandas**: For dataset loading, cleaning, and statistical summaries.
* **NumPy**: For array and numerical calculations.
* **Matplotlib**: For generating continuous and categorical visualizations.

## How to Run
1. Clone this repository to your local machine.
2. Ensure the dataset is located at `src/heart.csv` relative to the notebook.
3. Run the Jupyter Notebook (`heart_disease_analysis.ipynb`) sequentially to view the data processing, correlation matrices, and final insights.

## Let's Connect
* **LinkedIn**: [Let's network!](https://www.linkedin.com/in/mohammad-amin-saeini)
* **Kaggle**: [Check out on Kaggle!](https://www.kaggle.com/code/mohammadaminsaeini/heart-disease-analysis)
