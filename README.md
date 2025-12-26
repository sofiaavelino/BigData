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
   ```

2. Create a Python environment
   ```bash
   python -m venv venv
   source venv/bin/activate  # macOS/Linux
   venv\Scripts\activate     # Windows
   ```

3. Install packages
   ```bash
   pip install -r requirements.txt
   ```

4. Open the notebook
  ```bash
  jupyter notebook Project2_BDCC_GroupP.ipynb
  ```

### 📌 Option B — Google Colab
You can open the notebook with Colab (ideal if you don’t want to install locally):

👉 https://colab.research.google.com/github/sofiaavelino/BigData/blob/main/Project2_BDCC_GroupP.ipynb

## 📈 Key Results

- **Best performing model:**  
  Across all four illness groups, **XGBoost consistently outperformed other models** in terms of predictive accuracy for hospital length of stay (LOS).

- **Prediction accuracy:**  
  The models achieved a **mean absolute error (MAE) of approximately 2 days**. While not ideal, this performance is considered reasonable given:
  - the complexity of LOS prediction,
  - the limited size of the dataset,
  - and the high variability inherent in clinical data.

- **Computational performance:**  
  - **Sequential implementations** were faster than parallel approaches in both training and prediction time.
  - This is attributed to the dataset size being insufficient for parallelization benefits to outweigh overhead costs.
  - When comparing **Dask and PySpark**, execution time depended mainly on the chosen model rather than the framework itself, making it difficult to conclusively favor one over the other.

- **Practical relevance:**  
  - The predictions are **more informative for longer hospital stays** and more severe cases.
  - For short-term admissions, the added value of the predictions is limited.

- **Methodological insight:**  
  The results highlight the importance of **model selection and computational efficiency** in healthcare analytics, where timely and reasonably accurate predictions can support resource allocation and care planning.

- **Future directions:**  
  A promising extension would be **item-level temporal modeling**, where individual medical variables are modeled over time. While potentially more accurate and interpretable, this approach was deemed too complex and time-consuming for the scope of this project.




   
