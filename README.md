# Predictive Modeling for Diabetes Diagnosis
# Project Overview
This project explores the application of Machine Learning in Public Health screening. Using the Pima Indians Diabetes Dataset (N=768),I built and cpmpared two AI models to predict the onset of diabetes based on diagnostic measures like Glucose, BMI, and Age.
# Key Objectives
Data Processiing: Handling missing values and standardizing clinical features.
Modeling Comparison: Evaluating Logistic Regression vs. Random Forest to determine the best fit for small clinical datasets.
Safety Analysis: Analysing False Negatives (missed diagnoses) using Confusion Matrics to assess clinical risk.
# Key Findings
I tested two distinct alforithms to maximize diagnostic accuracy:
Model | Accuracy | False Negatives | Verdict
Logistic Regression | 74.7% | 18 | Selected |
Random Forset | 72.1% | 21 | Rejected |
Insights: The simpler model (Logistic Regresion) outperformed the complex Random Forest on this specific dataset. The Random Forest likely overfitted due to the small sample size, leading to more missed diagnosis (21 vs 18). From a Public Health perspective, the Logistic Regression is the safer, more robust choice here.
# Tech Used
Python: Analysis and Logic
Pandas: Data Manipulation
Scikit-Learn: Machine Learning Training 
Seaborn/Matplotlib: Heatmaps and Visualization
# Clinical Relevance
While the model achieved 75% accuracy, the analysis of the Confusion Matrix highlights the importance of Recall. In a real-worls setting, this tool would serve as a pre-screeing aid for nurses, flagging high-risk patients for further bloodwork, rather than a standalone diagnostic tool.
