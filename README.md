
---

# 🏦 Credit Risk Modeling (PD, LGD & EAD Estimation)

This repository contains a complete **Credit Risk Modeling** framework that estimates the **Probability of Default (PD)** and aligns with **IFRS 9** credit risk requirements.
It demonstrates how banks and financial institutions can quantify borrower creditworthiness and potential default exposure using machine learning.

---

##  Project Overview

This project simulates the end-to-end process of developing credit risk models:

* Estimating **PD (Probability of Default)** using logistic regression
* Preparing the foundation for **LGD (Loss Given Default)** and **EAD (Exposure at Default)** modeling
* Supporting **Expected Credit Loss (ECL)** computation under **IFRS 9**

It uses both **synthetic data generation** and **historical loan data** for demonstration and validation.

---

##  Workflow Summary

1. **Data Preparation**

   * Loan-level dataset (`loan_data.csv`) loaded and cleaned
   * Binary target (`default`) created from `loan_status`
   * Feature–target separation and dataset splitting (`split_train_test.txt`)

2. **Feature Engineering & Preprocessing**

   * Missing value handling
   * Feature scaling and normalization
   * Correlation analysis between dependent and independent variables

3. **Model Building**

   * Logistic Regression for PD estimation (`PD_IFRS.ipynb`)
   * Model evaluation using AUC, ROC, precision, recall, F1-score
   * Visualization of ROC curve and default distribution

4. **IFRS 9 Integration**

   * Framework compatible with PD, LGD, and EAD computation
   * IFRS-aligned PD modeling documented in `PD_Model.txt`

---

##  Example Metrics

| Metric                 | Description                                          |
| ---------------------- | ---------------------------------------------------- |
| **Accuracy**           | Overall model correctness                            |
| **AUC-ROC**            | Discrimination ability between default & non-default |
| **Precision / Recall** | Default prediction quality                           |
| **Confusion Matrix**   | Misclassification analysis                           |

---

##  Project Structure

```
PD_LGD_EAD_MODELING_IN-PYTHON_/
│
├── credit risk.ipynb                      # Exploratory analysis
├── credit risk2.ipynb                     # Model testing & improvements
├── PD_IFRS.ipynb                          # IFRS 9 aligned PD model
├── loan_data.csv                          # Loan-level dataset
├── PD_Model.txt                           # Model explanation and logic
├── split_train_test.txt                   # Data splitting script
├── Classification_Metrics_Explained.docx  # Model evaluation notes
├── dependent var code.txt                 # Target variable creation code
├── LICENSE
└── README.md
```

---

##  Tech Stack

* **Languages & Tools:** Python, NumPy, Pandas, Scikit-learn, Matplotlib, Seaborn
* **Modeling:** Logistic Regression (PD), ROC-AUC evaluation
* **Concepts:** Credit Risk, IFRS 9, PD/LGD/EAD, Expected Credit Loss
* **Environment:** Jupyter Notebook, VS Code

---

##  Future Enhancements

* Add **LGD** and **EAD** estimation modules
* Integrate **MLflow** for experiment tracking
* Deploy PD model via **FastAPI / Streamlit**
* Automate end-to-end modeling pipeline

---

## 👨‍💻 Author

**Gaurav Kumar**
📧 [hindugauravprataplahotiya@gmail.com](mailto:hindugauravprataplahotiya@gmail.com)
🔗 [GitHub Profile](https://github.com/Gaurav9693089415)

---

Would you like me to make a **shorter “resume version” summary** (2–3 lines with tech stack + link) for this project next — formatted just like your “DeepSeek” or “MLOps” entries?
