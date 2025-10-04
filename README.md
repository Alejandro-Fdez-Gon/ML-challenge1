#  SME Loan Approval Prediction Challenge  

This repository contains my participation in a **Machine Learning competition** based on a real-world problem: predicting whether a **Small and Medium-sized Enterprise (SME)** should be granted a loan or not.  

The task simulates the role of a bank officer who needs to assess the risk of granting a loan to a given company.  

## 📌 Problem Statement  
Given a dataset of SME enterprises that have applied for a loan, the goal is to **build a classifier that determines whether a loan should be approved or denied**.  

As a bank representative, the key question is:  
👉 *Should I grant a loan to Company X? Why or why not?*  

This decision is made by assessing the risk using historical loan application data.  

## 📊 Evaluation Metric  
The competition is evaluated using **Macro F1-Score**, which balances **precision** and **recall**.  

- **Precision (p):** Ratio of true positives to all predicted positives.  
- **Recall (r):** Ratio of true positives to all actual positives.  
- **Macro-F1:** Gives equal weight to each class, making it suitable for imbalanced datasets.  

## 📂 Dataset Description  

The dataset consists of information about companies applying for loans, including financial, geographic, and temporal attributes.  

**Files provided:**  
- `train.csv` → Training data with features + target (`Accept`).  
- `test_nolabel.csv` → Test data (without target).  
- `sample_submission.csv` → Example format for submission.  

**Main Features:**  
- `LoanNr_ChkDgt` → Loan petition identifier  
- `City`, `State`, `Bank`, `BankState` → Location and bank info  
- `ApprovalDate`, `DisbursementDate`, `ChgOffDate` → Temporal features  
- `NoEmp`, `CreateJob`, `RetainedJob` → Employment impact  
- `RevLineCr`, `LowDoc` → Loan program attributes  
- `DisbursementGross`, `BalanceGross` → Financial amounts  
- `Accept` → **Target variable** (0 = Not Approved, 1 = Approved)  

## 🗂️ Project Structure  

The workflow has been divided into several Jupyter notebooks:  

1. **`1_Carga_limpieza_datos.ipynb`** → Data loading & cleaning  
2. **`2_Visualizacion_datos.ipynb`** → Exploratory Data Analysis (EDA)  
3. **`3_Model_evaluation.ipynb`** → Baseline evaluation strategy  
4. **`4_Seleccion_caracteristicas_y_preprocesado.ipynb`** → Feature selection & preprocessing  
5. **`5_Entrenamiento_y_evaluacion_modelos.ipynb`** → Model training & evaluation  
6. **`6_Entrenamiento_y_evaluacion_nuevas_features.ipynb`** → Experiments with new engineered features  
7. **`7_Visualización_de_los_resultados.ipynb`** → Visualization of results & insights  
