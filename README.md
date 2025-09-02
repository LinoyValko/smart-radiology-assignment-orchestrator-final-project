# Smart Radiology Orchestrator: ML-Based Urgency Prediction for Medical Imaging

**B.Sc. Final Project – Digital Medical Technologies, HIT**

---

## Overview

This project was completed as part of a final undergraduate project at the Holon Institute of Technology (HIT) in collaboration with **Change Healthcare** (USA). The goal was to develop an AI-based decision support tool to assist radiologists in automatically prioritizing the interpretation of patient imaging exams, replacing the current manual “urgency” scoring system.

---

## Project Objectives

- Build a **machine learning model** to predict urgency scores based on patient exam data.
- Provide **explainable outputs** to align with clinical requirements.
- Enable **client-specific integration** by using both real and synthetic datasets.
- Optimize and automate the **workflow for radiologists**.

---

## Project Structure

### 1. `Data_Generation.ipynb`  
**Goal**: Generate synthetic data simulating real-world radiology exams.  
**Details**:
- Used probability distributions and feature ranges provided by Change Healthcare.
- Simulated fields include demographics, modality, exam type, and initial urgency.

---

### 2. `Atlantic_&_Avera.ipynb`  
**Goal**: Load and explore real de-identified datasets from two client hospitals: Atlantic and Avera.  
**Details**:
- Data loading, cleaning, and basic preprocessing.
- Initial feature analysis and outcome distribution.
- Validation of schema consistency and class balance.

---

### 3. `Hierarchical_Model.ipynb`  
**Goal**: Build a hierarchical grouping model to cluster patient exams based on shared features.  
**Details**:
- Used unsupervised learning (clustering) to group similar exams.
- Aimed to identify patient subgroups for downstream modeling.
- Helps uncover structure in data **without relying on predefined urgency rules**.

---

### 4. `Models.ipynb`  
**Goal**: Train ML models to predict urgency score.  
**Details**:
- Trained regression and classification models (e.g., Logistic Regression, Random Forest).
- Performed cross-validation and model evaluation using precision, recall, accuracy.
- Added explainability via feature importance and SHAP values.
- Final models are ready for production use by Change Healthcare.

---

## Technologies Used

- Python 3  
- NumPy, Pandas  
- Scikit-learn  
- Seaborn, Matplotlib  
- SHAP (for model explainability)  

---

## Deliverables

- Trained urgency score prediction models  
- Hierarchical grouping algorithm  
- Synthetic data generator  
- Ready-to-integrate pipeline for Change Healthcare systems

---

## 🤝 Acknowledgments

Special thanks to the **Change Healthcare** team for data support and domain insights, and to the faculty of **HIT’s Department of Digital Medical Technologies** for academic supervision.

---
