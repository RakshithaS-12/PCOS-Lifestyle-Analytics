# Explainable AI-Based PCOS Lifestyle Analytics

## 1. Project Overview

This project focuses on using Machine Learning and Explainable Artificial Intelligence (XAI) to classify lifestyle profiles and support personalized lifestyle recommendations for individuals with Polycystic Ovary Syndrome (PCOS).

The system analyzes lifestyle-related factors such as diet, exercise, sleep, stress, BMI, and menstrual cycle regularity to identify areas that may need attention.

Machine Learning classification algorithms are used to classify lifestyle profiles, while SHAP (SHapley Additive exPlanations) is used to understand the factors influencing model predictions.

## 2. Project Objectives

- Analyze lifestyle-related factors associated with PCOS management.
- Develop Machine Learning classification models.
- Compare different classification algorithms.
- Identify important lifestyle factors influencing predictions.
- Apply Explainable AI techniques using SHAP.
- Support personalized and explainable lifestyle guidance.

## 3. Dataset Description

The project uses a synthetically generated dataset named `PCOS_Lifestyle_Data.csv`.

**Dataset Details:**

- Total Records: 1,500
- Total Columns: 22
- Model Input Features: 19
- Target Variable: `Overall_Lifestyle_Profile`
- Missing Values: None
- Duplicate Records: None

**Target Classes:**

1. Generally Healthy
2. Some Areas Need Attention
3. Several Areas Need Attention

The dataset contains numerical and categorical lifestyle-related features.

**Important Note:** The dataset is synthetic and does not contain real patient records. The target labels were generated using predefined rules.

## 4. Technologies and Tools

- **Programming Language:** Python
- **Development Environment:** Google Colab
- **Version Control:** Git
- **Repository Hosting:** GitHub

## 5. Python Libraries

| Library | Purpose |
|---|---|
| Pandas | Data manipulation and analysis |
| NumPy | Numerical computations |
| Matplotlib | Data visualization |
| Seaborn | Statistical data visualization |
| Scikit-learn | Data preprocessing, model training and evaluation |
| SHAP | Explainable AI and model interpretation |

## 6. Methodology

The project follows these steps:

1. Dataset loading and exploration.
2. Data cleaning and preprocessing.
3. Feature selection.
4. Categorical feature encoding using OneHotEncoder.
5. Numerical feature scaling using StandardScaler.
6. Stratified train-test split (80:20).
7. Training multiple Machine Learning models.
8. Model evaluation and comparison.
9. SHAP-based explainability analysis.

## 7. Machine Learning Models

Three classification algorithms were implemented and compared:

- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier

**Final Model Selected:** Logistic Regression

Logistic Regression was selected based on its overall evaluation performance.

## 8. Model Evaluation

The final Logistic Regression model achieved the following results on the test dataset:

| Evaluation Metric | Score |
|---|---:|
| Accuracy | 94.67% |
| Macro Precision | 95.02% |
| Macro Recall | 91.19% |
| Macro F1-Score | 92.97% |

These results represent the model's performance on the test split of the synthetic dataset.

## 9. Explainable AI Using SHAP

SHAP (SHapley Additive exPlanations) was used to interpret the Machine Learning model and identify the features contributing to its predictions.

The following features showed higher global SHAP importance:

| Feature | SHAP Importance |
|---|---:|
| Exercise | 1.8917 |
| Period Regularity | 1.7713 |
| Diet | 1.7475 |
| Sleep | 1.4797 |
| Stress | 1.4487 |
| BMI | 0.2197 |
| Daily Activity | 0.2006 |
| Cycle Length | 0.1966 |
| Excess Hair | 0.1826 |
| Water Intake | 0.1648 |

The results indicate that exercise, period regularity, diet, sleep, and stress were among the most influential features in the model's predictions.

SHAP explains the model's behavior; it does not establish causal relationships.

## 10. Repository Structure

```text
PCOS-Lifestyle-Analytics/
│
├── PCOS_Lifestyle_Analytics.ipynb
├── PCOS_Lifestyle_Data.csv
├── README.md
└── .gitignore
```

## 11. Limitations

- The dataset is synthetically generated and does not represent real patient data.
- The model has not undergone clinical validation.
- Model performance on synthetic data does not guarantee similar performance on real-world data.
- SHAP explains model predictions but does not establish cause-and-effect relationships.
- The system is not designed to diagnose PCOS.

## 12. Disclaimer

This project is developed for academic and educational purposes. It demonstrates the application of Machine Learning and Explainable AI techniques for lifestyle profile classification and PCOS-related lifestyle support.

The predictions and recommendations are not a substitute for professional medical advice, diagnosis, or treatment.

## 13. Author

**Rakshitha Shetty**

MSc Information Technology

**Project Title:** Explainable AI-Based Personalized Lifestyle Recommendation System for Polycystic Ovary Syndrome (PCOS) Management
