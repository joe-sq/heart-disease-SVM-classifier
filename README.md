# Heart Disease Prediction using SVM ❤️📊

An end-to-end machine learning project that analyzes clinical data and predicts the likelihood of heart disease in patients using a Support Vector Machine (SVM) classifier. 

## 📌 Project Overview
Cardiovascular diseases are the leading cause of death globally. This project leverages Python and Scikit-Learn to build a predictive model based on patient medical records. It includes comprehensive Exploratory Data Analysis (EDA) to uncover trends—such as the relationship between high blood pressure and heart disease—followed by feature scaling and classification.

## 🗂️ Dataset Attributes
The dataset (`heart.csv`) contains 918 patient records with the following features:
* **Age:** Patient's age in years
* **Sex:** Gender (M: Male, F: Female)
* **ChestPainType:** TA (Typical Angina), ATA (Atypical Angina), NAP (Non-Anginal Pain), ASY (Asymptomatic)
* **RestingBP:** Resting blood pressure in mm Hg
* **Cholesterol:** Serum cholesterol in mg/dL
* **FastingBS:** Fasting blood sugar > 120 mg/dL (1 = True, 0 = False)
* **RestingECG:** Resting electrocardiogram results (Normal, ST, LVH)
* **MaxHR:** Maximum heart rate achieved (bpm)
* **ExerciseAngina:** Exercise-induced angina (Y = Yes, N = No)
* **Oldpeak:** ST depression induced by exercise relative to rest
* **ST_Slope:** The slope of the peak exercise ST segment (Up, Flat, Down)
* **HeartDisease:** Target class (1 = Heart Disease, 0 = Normal)

## 🛠️ Project Workflow
1. **Data Loading & Inspection:** Read the dataset and check features, data types, and null values.
2. **Exploratory Data Analysis (EDA):**
   * Calculated the mean age of patients.
   * Plotted Age Distribution (Histogram).
   * Visualized Gender Distribution (Bar Chart).
   * Analyzed Heart Disease rates in patients with High Blood Pressure (> 170).
   * Plotted Cholesterol Distribution (Histogram).
3. **Data Preprocessing:** * Isolated the numerical predictive features (`Age`, `RestingBP`, `Cholesterol`, `FastingBS`, `MaxHR`, `Oldpeak`).
   * Split the data into training (80%) and testing (20%) sets.
   * Applied `StandardScaler` to normalize the feature distributions.
4. **Model Training:** Initialized and trained a Support Vector Classifier (`SVC`).
5. **Evaluation:** Tested the model against the holdout set, achieving an **accuracy of ~78.26%** (exceeding the 70% baseline requirement).
6. **Interactive Prediction:** Includes a script to input custom patient data and receive a real-time prediction.

## 💻 Technologies Used
* **Python 3.x**
* **Pandas:** Data manipulation and analysis
* **Matplotlib:** Data visualization
* **Scikit-Learn:** Data scaling (`StandardScaler`), Model training (`SVC`), and evaluation (`accuracy_score`)
* **Jupyter Notebook:** Interactive development environment
