# HealthyBite-Predictor

### Project Overview

The aim of this project is to determine whether machine learning algorithms can consistently estimate Nutri-Score values of food products (A-E) based on information from an OpenFoodFacts dataset which includes standardised Nutritional Information about these products. Although Nutri-Score provides a simple way to tell consumers about their nutritional intake, it is often not available for every single food product, nor is it always shown on food packaging in the same way in different areas or countries. Therefore, the opportunity exists to produce a Nutri-Score value for any product using the nutrient-containing raw data.

The project uses an end-to-end machine learning pipeline built around the raw Nutritional Information dataset, as well as methods for cleaning and preparing the data such as removing unneeded information, dealing with missing values, feature engineering and scaling the data prior to developing and evaluating models.

A variety of models were evaluated with this data set starting with a logistic regression model which served as the baseline model; in addition, several tree-based methods including Random Forest, XGBoost, LightGBM, and a stacking ensemble built upon these tree-based methods were constructed. The results of this project demonstrate that tree-based models produce very good accuracy and have strong generalisability, thereby providing additional evidence to support the conclusion that Nutri-Score can be reliably predicted from nutrient content alone. The findings in this research also highlight the potential role for machine learning in providing consumers with consistent nutrition guidance with regards to food products that do not have adequate front-of-package labelling.
