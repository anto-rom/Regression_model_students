Student Academic Performance Prediction
Overview

This project aims to predict students’ academic performance based on variables related to study habits, attendance, sleep patterns, and learning styles.
The analysis was carried out from two complementary perspectives:

Classification: Predict whether a student will pass or fail.

Regression: Predict the student’s final grade.

The dataset includes information from 1,000 students, combining numerical and categorical variables that reflect academic behavior and engagement.

Project Objectives

Identify the factors with the strongest impact on student performance.

Develop predictive models for both classification and regression tasks.

Evaluate performance through standard metrics and ensure model stability.

Provide interpretable insights to support data-driven educational strategies.

Dataset Structure
Variable Type	Columns
Numerical	horas_estudio_semanal, nota_anterior, tasa_asistencia, horas_sueno, edad, nota_final
Categorical	nivel_dificultad, tiene_tutor, horario_estudio_preferido, estilo_aprendizaje
Target Variables	aprobado (binary), nota_final (continuous)
Methodology

Exploratory Data Analysis (EDA):

Distribution analysis, correlations, and outlier detection.

Relationship between study patterns and final performance.

Preprocessing:

Missing value imputation (median/mode).

OneHotEncoder for categorical features.

Standardization of numerical variables.

Predictive Modeling:

Classification: Logistic Regression and Random Forest Classifier.

Regression: Linear Regression and Random Forest Regressor.

80/20 train-test split and metric-based model evaluation.

Evaluation & Validation:

Classification → Accuracy, F1, ROC-AUC.

Regression → MAE, RMSE, R².

Residual analysis and model comparison.

Key Results
Classification Model (Pass/Fail)

Accuracy: 0.85 – 0.90

F1-score: 0.84

ROC-AUC: 0.90

Top Predictors: nota_anterior, tasa_asistencia, horas_estudio_semanal, tiene_tutor.

Regression Model (Final Grade)

R²: 0.82 – 0.88

MAE: 0.35 – 0.45

RMSE: 0.50

Top Predictors: nota_anterior, tasa_asistencia, horas_sueno.

Conclusions

Academic success is primarily driven by prior performance, attendance, and consistent study habits.

The variable nota_anterior (previous grade) consistently emerges as the strongest predictor across both models.

Random Forest models provided a better trade-off between accuracy and robustness.

The predictive system can be used to detect at-risk students and anticipate early intervention needs.

Next Steps

Optimize hyperparameters via GridSearchCV.

Implement model explainability tools such as SHAP or LIME.

Enrich the dataset with behavioral variables (participation, motivation, assignment submission).

Integrate the model into a real-time academic monitoring dashboard.

Technologies Used

Python 3.x

Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, SciPy

Jupyter Notebook / VS Code

Author

Antonio Romero
Continuous Improvement & VoC Team Leader
Responsible for data analysis, model development, and documentation.
