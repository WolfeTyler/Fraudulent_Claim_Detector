# Fraudulent Claim Detection ML Project

> A machine learning project to analyze and detect fraudulent insurance claims using logistic regression and random forest classifiers.

## Table of Contents

* [General Information](#general-information)  
* [Technologies Used](#technologies-used)  
* [Conclusions](#conclusions)  
* [Acknowledgements](#acknowledgements)  
* [Contact](#contact)  

## General Information

* **Objective:** Build and evaluate models that can flag potentially fraudulent insurance claims, helping insurers reduce financial losses and streamline investigation workflows.  
* **Business Problem:** Manual review of every claim is time‑consuming and costly. An automated fraud‑detection pipeline can prioritize high‑risk cases for further investigation.  
* **Dataset:** The provided `Fraudulent_Claim_Detection_Starter.ipynb` notebook ingests an insurance‑claims dataset containing policy details, claimant demographics, incident descriptions, coverages, and a binary target (`fraud_reported`).  
* **Reproduction:** To reproduce the analysis end‑to‑end, open and run the Jupyter notebook. You’ll see data preprocessing, feature selection, model training (logistic regression & random forest), cutoff optimization, and validation steps.

## Technologies Used

* **Python 3.x**  
* **pandas** for data manipulation  
* **numpy** for numerical operations  
* **scikit‑learn** for model building, evaluation, and hyperparameter tuning  
* **imbalanced‑learn** for handling class imbalance (oversampling)  
* **matplotlib** & **seaborn** for plotting (ROC, precision‑recall, confusion matrices)  

## Conclusions

* **Logistic Regression:**  
  * After L1‑based feature selection and cutoff optimization, achieved balanced precision/recall on the validation set.  
  * Key drivers of fraud included features such as `collision_type`, `property_damage`, `incident_severity`, and claimant injury descriptions.  

* **Random Forest:**  
  * Hyperparameter tuning (via grid search) further improved F1‑score over the logistic baseline.  
  * Cross‑validation showed minimal overfitting, with training and validation accuracies closely aligned.  

* **Precision–Recall Trade‑off:**  
  * The chosen probability cutoff balances the need to catch as many frauds as possible (high recall) while keeping false‑positive rates manageable (precision).

## Acknowledgements

* Starter notebook and dataset provided as part of the project assignment.  
* Documentation and tutorials from the scikit‑learn and imbalanced‑learn libraries.  
* Inspiration from real‑world fraud‑detection case studies in insurance.

## Contact

Created by [@WolfeTyler](https://github.com/WolfeTyler). Feel free to open an issue or reach out with questions or feedback!  
