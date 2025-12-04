# STAT432 Final Project: Glioma Grading Classification

> **Every year, thousands of patients face a critical diagnosis: is their brain tumor slow-growing or aggressively lethal?** This project leverages machine learning to distinguish between low-grade gliomas (LGG) and glioblastomas (GBM), enabling faster, more accurate diagnoses that could save lives.

## Project Overview

This project develops and evaluates classification models to predict brain tumor grades using clinical and genetic features from The Cancer Genome Atlas (TCGA). Gliomas are the most common primary brain tumors, and accurately differentiating between LGG and GBM is critical for optimizing treatment strategies, reducing toxicity, and improving survival rates.

### Key Objectives
- **Build robust classification models** to predict tumor grade (LGG vs. GBM)
- **Identify the most impactful genetic and clinical features** for prediction
- **Compare model performance** across six different machine learning approaches

### Dataset
- **Source**: TCGA Glioma Grading Clinical and Mutation Features (UCI ML Repository)
- **Size**: 862 observations
- **Features**: 20 gene mutations + 3 clinical variables (Age, Gender, Race)
- **Target**: Binary classification (LGG vs. GBM)

### Models Implemented
1. K-Nearest Neighbors (KNN)
2. Logistic Regression
3. Random Forest
4. Gradient Boosting (GBM)
5. AdaBoost
6. Support Vector Machine (SVM)

### Key Results
- **Most important features**: IDH1, Age at Diagnosis, TP53, ATRX, and EGFR mutations
- All models achieved **>80% accuracy** with strong sensitivity for GBM detection

### Technologies Used
- **Language**: R
- **Key Libraries**: `tidyverse`, `caret`, `randomForest`, `gbm`, `e1071`, `pROC`
- **Analysis**: Cross-validation, hyperparameter tuning, ROC/AUC evaluation

---

## Folder Structure
* **`data/`** - Raw datasets from TCGA (mutations and clinical information)
* **`doc/`** - R Markdown analysis file (`STAT432Project.Rmd`) and final report PDF (`STAT_432_REPORT.pdf`)
* **`misc/`** - Visualizations, diagnostic plots, and supplementary figures



## Authors
- **Karina Grewal** 
- **Steve Liang**  

---

*For detailed methodology, results, and discussion, please refer to [`doc/STAT_432_REPORT.pdf`](doc/STAT_432_REPORT.pdf).*
