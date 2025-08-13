# Heart Disease Prediction using Logistic Regression  

## 📌 Project Overview  
This project uses **Logistic Regression** to predict the likelihood of heart disease in patients based on various medical attributes. Logistic Regression is a statistical method suitable for binary classification problems, making it ideal for predicting whether a patient has heart disease (`1`) or not (`0`).  

The dataset used contains patient health records with features such as age, sex, cholesterol levels, blood pressure, and other cardiovascular indicators.  

---

## 🗂 Dataset  
The dataset includes the following features:  

- **Age** – Age of the patient (years)  
- **Sex** – Gender (1 = male, 0 = female)  
- **cp** – Chest pain type (categorical: 0–3)  
- **trestbps** – Resting blood pressure (mm Hg)  
- **chol** – Serum cholesterol level (mg/dl)  
- **fbs** – Fasting blood sugar > 120 mg/dl (1 = true, 0 = false)  
- **restecg** – Resting electrocardiographic results (0–2)  
- **thalach** – Maximum heart rate achieved  
- **exang** – Exercise-induced angina (1 = yes, 0 = no)  
- **oldpeak** – ST depression induced by exercise relative to rest  
- **slope** – Slope of the peak exercise ST segment  
- **ca** – Number of major vessels colored by fluoroscopy (0–3)  
- **thal** – Thalassemia status (categorical: 0–3)  
- **target** – Heart disease diagnosis (1 = disease, 0 = no disease)  

---

## ⚙️ Project Workflow  

1. **Import Libraries**  
   - `pandas`, `numpy` for data manipulation  
   - `matplotlib`, `seaborn` for visualization  
   - `sklearn` for model training, evaluation, and preprocessing  

2. **Data Exploration**  
   - Checked dataset shape, null values, and statistical summaries  
   - Explored distributions of target and features  
   - Visualized correlations using heatmaps and pair plots  

3. **Data Preprocessing**  
   - Handled missing values  
   - Encoded categorical features  
   - Standardized numerical features  

4. **Model Building**  
   - Implemented **Logistic Regression** from `sklearn.linear_model`  
   - Split data into **training** and **testing** sets (80:20)  
   - Trained the model on the training dataset  

5. **Model Evaluation**  
   - Accuracy Score  
   - Confusion Matrix  
   - Classification Report (Precision, Recall, F1-score)  
   - AUC-ROC Score  

---

## 📊 Results  

| Metric              | Score  |
|---------------------|--------|
| **Accuracy**        | 0.7869 |
| **Precision (avg)** | 0.79   |
| **Recall (avg)**    | 0.78   |
| **F1-score (avg)**  | 0.78   |
| **AUC-ROC Score**   | 0.8647 |

**Confusion Matrix:**  

[[19 9]
[ 4 29]]

**Class-wise performance:**  
- Class `0` (No Heart Disease): Precision = 0.83, Recall = 0.68, F1 = 0.75  
- Class `1` (Heart Disease): Precision = 0.76, Recall = 0.88, F1 = 0.82  

---
