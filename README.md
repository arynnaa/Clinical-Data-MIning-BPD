CLINICAL DATA MINING: Predicting Bronchopulmonary Displasia (BPD)

 Project Overview: 
This project explores clinical and perinatal factors associated with bronchopulmonary dysplasia (BPD) in very-low-birth-weight (VLBW) infants. 
The analysis uses the PreMo dataset to examine relationships between selected demographic and perinatal charateristics and BPD status at 36 weeks postmentstrual age. Several machine learning classification models are developed and compared to evaluate their performance in predicting BPD status. 

Objectives: 
- Prepare and preprocess the clinical dataset for analysis.
- Explore differences in selected characteristics between infants with and without BPD. 
- Build and compare classification models for BPD status prediction. 
- Examine feature importance to identify variables that contribute to model predictions. 
- Discuss model performance, limitations, and potential directions for future research. 

Dataset: 
The project uses the PreMo clinical dataset, which contains demographic, perinatal, and clinical outcome information. 
The target variable is bpd_36_weeks. 

The analytical sample includes 3,917 infants with known BPD status after data preparation and exclusion of records with unknown or missing target values. The dataset is not included in this repository by default. Please refer to the original dataset source and its access and usage conditions before obtaining or redistributing the data. 

Methodology: 
The analysis includes the following steps: 

1. Data preparation: Merge the demographic and perinatal data with discharge and outcome information. 
2. Exploratory data analysis (EDA): Examine the distribution of BPD status and relationships between the outcome and selected variables.  
3. Preprocessing: Handle missing values using median imputation for numerical variables and most-frequent-category imputation for categorical variables. Apply feature scaling and one-hot encoding when appropriate. 
4. Model development: Train nd compare the following classification models: 
   - Logistic Regression 
   - Decision Tree 
   - Random Forest 
   - XGBoost 
5. Evaluation: Compare model performance using accuracy, precision, recall, F1-score, and ROC-AC. 
6. Interpretation: Examine XGBoost feature importance to explore which variables contribute to the model's predictions. 
Preprocessing is performed within a machine learning pipeline to help prevent data leakage. The data is split into training and testing sets using an 80:20 ratio with stratification. 

Tools and Technologies: 
- Python
-Pandas and NumPy
-Matplotlib and Seaborn
-Scikit-learn
-XGBoost 
-Google Colab/ Jupyter Notebook

Results Summary: 
Logistic Regression achieved the highest ROC-AUC among the four evaluated models, at 67.39%. It also achieved an accoracy of 63.39%.  The results indicate that distinguishing between infants with and without BPD is a challenging classification task using the selected predictors. Model performance varied across evaluation metrics, and no single model performed best on every metric. The analysis also illustrates the importance of controlling overfitting and interpreting feature importance carefully. 

Limitations: 
- The analysis uses selected demographic and perinatal variables rather than the full range of potentially relevant clinical information. 
- Predictive performance indicates model relies on variables; it does not establish causation. 
- The findings should not be interpreted as clinical advice or as a validated clinical prediction tool. 

Repository Contents: 
- PreMo_BPD_Data_Mining_Analysis.ipynb notebook containing the data analysis, preprocessing model training, evaluation, and visualizations. 
- README.md is a project overview, methodology, results, and limitations. 

The dataset is not included by default and must be accessed separately in accordance with its applicable terms. 

Disclaimer: 

This project was completed as an academic data mining study. It is intended for educational and analytical purposes inly and it is not intended for clinical decision making. 
