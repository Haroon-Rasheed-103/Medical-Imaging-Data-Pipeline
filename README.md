(Model which did not give good results)
# 🏥 Medical Imaging & Clinical Data Integration Pipeline

## 📌 Project Overview
This repository contains the data engineering layer and processing infrastructure for my **Final Year University Project**. The objective of this system is to ingest, clean, and unify two completely different data types—unstructured volumetric medical images and structured clinical text profiles—into a single, high-performance training pipeline for predictive care.

---

### 🏗️ Architecture & Engineering Flow

[ Raw Images ]      ---> [ Image Transformation Layer ] 
---> [ Unified Feature Matrix ] ---> [ ML Pipeline ]
[ Clinical Records ] ---> [ Schema Cleaning & Encoding ] /

1. **Structured Ingestion Layer:** Imports raw patient records, addresses missing health markers, and applies categorical encoding using Pandas.
2. **Unstructured Ingestion Layer:** Imports raw lungs imaging data, handles noise reduction, and applies image pre-processing matrices so pixel grids match.
3. **The Multi-Modal Join:** Merges disparate imaging features and text records together based on unique indexing keys without dropping data variance.
4. **Validation Pipeline:** Feeds the synchronized arrays into an isolated machine learning evaluation script.

---

### 🛠️ Technical Stack
* **Language:** Python
* **Data Processing:** Pandas, NumPy
* **Machine Learning Infrastructure:** Scikit-Learn
* **Environment:** Jupyter Notebooks & Structured Python Scripts
