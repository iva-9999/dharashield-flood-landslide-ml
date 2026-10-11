# DharaShield 🛡️

DharaShield is an end-to-end village-level flood and landslide early warning system designed for India's hilly regions. Built by **Team ResQNova** for **Smart India Hackathon (SIH) 2026** (Problem Statement 26192, Ministry of Home Affairs / National Disaster Response Force).

---

## 📌 The Problem & Our Solution
* **The Gap:** Traditional disaster management warnings in India are typically issued at the **district level**, which is too broad for mountainous terrain where micro-climates and village topography dictate risk.
* **The Solution:** DharaShield scores **each village individually** using two specialized Random Forest models (one for floods, one for landslides) trained on multi-source government and remote sensing data. Every prediction is paired with **SHAP (SHapley Additive exPlanations)** to provide transparent, explainable risk factors.

---

## 📊 Data Sources
Our models synthesize data from trusted national and global repositories:
* **NDEM** (National Database for Emergency Management)
* **GSI** (Geological Survey of India)
* **ISRO / NRSC** (Indian Space Research Organisation / National Remote Sensing Centre)
* **NASA SRTM** (Elevation and topography dataset)

---

## 🤖 Model Performance & Validation
* **Granularity:** Scores **3,08,983 villages** across target hill states.
* **Robustness Check:** The flood model was tested on three states withheld entirely from training (**Manipur, Meghalaya, and Tripura**), achieving an out-of-sample AUC between **0.826 and 0.992**.

---

## 🗂️ Project Structure
* `/dashboard` — Web dashboard for visualizing village risk scores and SHAP breakdowns.
* `/ml_pipeline` — Python scripts for data cleaning, feature engineering, and model training.
* `/docs` — Detailed model cards, architecture diagrams, and write-ups.
* `/results` — Model comparison metrics, SHAP plots, and feature importances.
* `/data` — Source references and schemas.

---

## 🏆 Team ResQNova
Built for Smart India Hackathon 2026.
