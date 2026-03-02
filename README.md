# 🌟 eCommerce Customer Support — CSAT Prediction (Machine Learning Project)

This project focuses on analyzing eCommerce customer support interactions and building a **machine learning classification model** to predict whether a customer is **Satisfied (1)** or **Not Satisfied (0)**.  
Since the provided dataset did not include an actual CSAT label, a **synthetic but meaningful target** was engineered for ML modeling, ensuring the project follows real-world practices.

---

## 📌 Project Overview

Customer support interactions contain valuable signals such as:
- Handling time  
- Issue categories  
- Agent performance  
- Customer remarks  
- Response delays  

By processing these variables, we can **predict customer satisfaction** and identify operational areas needing improvement.

---

## 🎯 Business Objective

To develop a machine learning model that predicts whether a customer is satisfied or dissatisfied based on support ticket information.  
This helps businesses:

- Reduce ticket handling time  
- Improve agent efficiency  
- Boost CSAT & NPS scores  
- Prioritize high-risk customers  
- Automate quality monitoring  

---

## 📁 Dataset Used

**Filename:** `eCommerce_Customer_support_data.csv`  
Contains features like:
- Channel name  
- Ticket categories  
- Customer remarks  
- Handling time  
- Response delay  
- Agent/supervisor details  

Since *CSAT was not included*, a synthetic binary CSAT label was generated for modeling.

---

## 🛠 Project Workflow

### **1️⃣ Exploratory Data Analysis (EDA)**
- Data cleaning  
- Missing value handling  
- Outlier treatment  
- Visualization using UBM Rule:
  - Univariate  
  - Bivariate  
  - Multivariate  

### **2️⃣ Feature Engineering**
- Word count from customer remarks  
- Handling time conversion  
- Delay time calculation  
- Encoding categorical variables  

### **3️⃣ Synthetic Target Creation**
Because the dataset had **no CSAT column**, a synthetic binary target (0/1) was created.  
This allowed meaningful ML modeling without breaking the project structure.

### **4️⃣ Model Building**
Models implemented:
- Logistic Regression  
- Decision Tree  
- Random Forest  

Class imbalance handled using **SMOTE**.

### **5️⃣ Evaluation Metrics**
- Accuracy  
- Precision  
- Recall  
- F1-score  
- Confusion Matrix  

### **6️⃣ Best Model**
**Random Forest Classifier** provided the best results and was saved as : models/best_model.pkl

---

## 📦 Folder Structure

📦 eCommerce-CSAT-ML-Project
┣ 📜 README.md
┣ 📜 requirements.txt
┣ 📂 data
┃ ┗ 📄 eCommerce_Customer_support_data.csv
┣ 📂 notebooks
┃ ┗ 📓 ML_Project.ipynb
┗ 📂 models
┗ best_model.pkl

---

## 🚀 How to Run the Project

pip install -r requirements.txt
jupyter notebook notebooks/ML_Project.ipynb

---

## 🔮 Future Improvements

- Add real CSAT labels if available
- Deploy model using Streamlit / Flask
- Add sentiment analysis (NLP) for customer remarks
- Build a real-time CSAT prediction dashboard

---

## 👩‍💻 Author

**Name**: ALVIRA PARVEEN  
🔗 [LinkedIn](https://www.linkedin.com/in/alvira-parveen-78022536b)  
🌐 [GitHub](https://github.com/Alvira-Parveen)
