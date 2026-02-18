# 🧬 Breast Cancer Classification using miRNA & Clinical Data (TCGA-BRCA)

![Python](https://img.shields.io/badge/Python-3.x-blue?style=flat&logo=python)
![Scikit-Learn](https://img.shields.io/badge/Library-Scikit--Learn-orange?style=flat&logo=scikit-learn)
![Bioinformatics](https://img.shields.io/badge/Domain-Bioinformatics-green)
![Status](https://img.shields.io/badge/Status-Research_Complete-success)

> **Lab:** Khayyam AI Innovation Lab  
> **Supervisor:** Dr. Saeed Pirmoradi  
> **Researcher:** Shayan Abdollahi Nami  
 

---

## 📖 Project Overview

This project investigates the potential of **miRNA expression profiles** combined with clinical data to predict **Lymph Node Metastasis (N0 vs N1)** in Breast Invasive Carcinoma using the **TCGA-BRCA** dataset from The Cancer Genome Atlas (TCGA).

MicroRNAs (miRNAs) are small non-coding RNAs that play a critical role in tumor progression and metastasis. This study applies statistical machine learning models to high-dimensional genomic data to identify robust predictive biomarkers.

---

## 🔬 Methodology & Pipeline

### 📊 Data Source
- TCGA-BRCA miRNA expression data (Isoform-level)
- Clinical supplement data
- Patient matching between genomic and clinical datasets

### 🧹 Preprocessing
- Data cleaning and filtering  
- Patient ID alignment  
- Feature standardization using `StandardScaler`

### 📉 Dimensionality Reduction
- **Principal Component Analysis (PCA)**
  - Visualization of class separability
  - Reduction of high-dimensional feature space

### 🤖 Classification Models
- **LDA** – Linear Discriminant Analysis  
- **QDA** – Quadratic Discriminant Analysis  
- **GNB** – Gaussian Naive Bayes  

---

## 📊 Results & Discussion

Models were evaluated on a held-out test set to assess generalization performance.

| Model | Performance | Key Insight |
|--------|------------|------------|
| **LDA** | 🏆 Most Stable | Best generalization with balanced training and test performance |
| **QDA** | Overfitting | Perfect training accuracy but weaker test performance due to high complexity |
| **GNB** | Baseline | Lower accuracy; independence assumption likely violated in miRNA data |

📉 Detailed confusion matrices and PCA visualizations are available in:

**Breast Cancer Report.pdf**

---

## 📂 Repository Structure

```text
TCGA-BRCA-miRNA-Analysis/
│
├── data/                       # [Required] Place TCGA miRNA & Clinical files here
│
├── BRCA_GNB_PCA_LDA_QDA.ipynb  # Main Analysis Notebook
├── Breast Cancer Report.pdf    # Official Lab Report (Khayyam AI Lab)
└── README.md                   # Documentation      

---


⚠️ Disclaimer
This project is conducted under the supervision of Khayyam AI Innovation Lab for academic research purposes. Results are computational and not for clinical diagnosis.





