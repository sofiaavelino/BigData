# BigData Analytics for Healthcare — Hospital LOS Prediction

**Predicting Length of Hospital Stay (LOS) using Big Data Analytics and Machine Learning in Healthcare**

This repository contains the final project for the *Big Data and Cloud Computing* course. The goal of this project is to apply big data analytics and machine learning techniques to a large clinical dataset (MIMIC-III) in order to predict patients’ **length of hospital stay (LOS)** and derive insights about factors influencing LOS.

---

## 🧠 Motivation

Healthcare systems generate vast amounts of data daily. Effective analysis of these datasets can help hospitals:

- Allocate resources more efficiently  
- Improve patient care planning  
- Reduce unnecessary costs  
- Support data-driven decision making  

Accurately predicting LOS can inform bed management, staffing, and discharge planning.

---

## 📊 Dataset

This project uses the **MIMIC-III clinical database**, which contains de-identified health data associated with ~40,000 ICU patients, including demographics, vitals, lab results, and more.

> **Note:** Due to privacy restrictions, MIMIC-III requires credentialed access from PhysioNet — describe how others can obtain the credentials and download the data.

---

## 📌 Project Overview

The core notebook, `Project2_BDCC_GroupP.ipynb`, performs:

1. Data loading and preprocessing  
2. Feature engineering  
3. Exploratory data analysis  
4. Model training (e.g., regression, random forest, etc.)  
5. Model evaluation and discussion of results

You can extend this analysis with other models or feature sets.

---

## 🧪 How to Run

### 📌 Option A — Local Jupyter

1. Clone the repository  
   ```bash
   git clone https://github.com/sofiaavelino/BigData.git
   cd BigData

2. Create a Python environment
   ```bash
   python -m venv venv
   source venv/bin/activate  # macOS/Linux
   venv\Scripts\activate     # Windows

3. Install packages
   ```bash
   pip install -r requirements.txt

4. Open the notebook
  ```bash
  jupyter notebook Project2_BDCC_GroupP.ipynb
  ```

### 📌 Option B — Google Colab
You can open the notebook with Colab (ideal if you don’t want to install locally):
👉 https://colab.research.google.com/github/sofiaavelino/BigData/blob/main/Project2_BDCC_GroupP.ipynb

### 📈 Key Results



   
