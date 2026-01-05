# HealthyBite-Predictor

### Project Overview

**Goal:**
Develop and evaluate machine learning models to predict Nutri-Score grades for packaged food products using nutritional and ingredient-level data, with an emphasis on model interpretability, data quality challenges, and generalization performance.

**Project Overview**
This repository contains a complete end-to-end machine learning pipeline for Nutri-Score prediction using the OpenFoodFacts database. The project covers data exploration, cleaning, feature engineering, model development, evaluation, and interpretation, with a focus on understanding how nutritional attributes influence food health ratings.

**Focus Areas Include**
- Nutritional quality assessment
- Nutri-Score grade classification (A–E)
- Feature engineering using macronutrients and derived ratios
- Model interpretability and generalization
- Handling real-world, noisy food labeling data

**Data**
Source:
- OpenFoodFacts (public, crowd-sourced food database)
Challenges:
- High missingness across many features
- Heavy-tailed and skewed distributions
- Multicollinearity among nutritional variables
- Moderate class imbalance across Nutri-Score grades

**Methods**
Models:
- Logistic Regression
- Random Forest
- XGBoost
- LightGBM
- Stacking Ensemble (RF + XGBoost + Logistic Regression)
Techniques
- Data cleaning with missingness thresholds and valid-range filtering
- Winsorization and RobustScaler for outlier handling
- Feature engineering and ratio construction
- Multicollinearity analysis (correlation heatmaps, VIF)
- Model comparison using accuracy, macro F1, ROC/AUC
- Overfitting analysis (train vs test performance)
- Model interpretability via feature importance and confusion matrices

**Key Results**
- **Best-performing models:** LightGBM and XGBoost
- **Overall performance:**
    - Test accuracy ≈ 0.98
    - Strong macro F1 across Nutri-Score classes
    - High multiclass ROC AUC with clear class separability
- **Most influential features:**
    - Salt
    - Energy
    - Sugars
    - Saturated fat
    - Fiber
    - Protein-to-energy ratio
- **Error patterns:**
    - Most misclassifications occur between adjacent Nutri-Score grades (e.g., B vs C, D vs E), which is consistent with the continuous nature of nutritional quality

**Tools & Technologies**
- Python (pandas, NumPy, scikit-learn)
- XGBoost, LightGBM
- matplotlib / seaborn
- Jupyter Notebook
- GitHub for version control and project organization

Repository Structure 
```
data/                 # Raw and processed datasets
notebooks/            # Data cleaning, modeling, evaluation notebooks
visualizations/
  Exploration_Cleaning/
  Cleaning_Modeling/
  Modeling/
report/               # Final written report
presentation/         # Slides summarizing findings
```

**Limitations & Future Work**
- OpenFoodFacts data quality depends on user-entered labels
- Limited availability of micronutrient and additive details for many products
- Nutri-Score is a simplified proxy for nutritional health
- Future extensions could include:
    - Ingredient text analysis using NLP
    - External validation on country-specific datasets
    - Calibration analysis for consumer-facing applications
    - SHAP-based local explanations for individual products

Tighten this into a shorter “portfolio-style” README

Rewrite it to sound more research-oriented or more industry-oriented

Align it exactly with a CDS 403 grading rubric
