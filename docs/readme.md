
# 👁️ Diabetic Retinopathy & Metabolic Risk Assessment

> **Explainable retina screening platform combining EfficientNet-B0 (Grad-CAM), U-Net lesion segmentation, and patient metabolic risk fusion into an interactive Streamlit dashboard.**

[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![PyTorch](https://img.shields.io/badge/PyTorch-2.0+-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)](https://pytorch.org)
[![Streamlit](https://img.shields.io/badge/Streamlit-Dashboard-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)](https://streamlit.io)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](#)

---

## 📌 Clinical Overview & Motivation

**Diabetic Retinopathy (DR)** is a major cause of microvascular ocular damage in diabetic patients. Traditional diagnostic tools often rely solely on retinal fundus scans, ignoring systemic patient markers or providing black-box predictions.

This project introduces a multi-modal screening suite that merges:
1. **Ocular Computer Vision:** Disease grading, Grad-CAM visual explainability, and lesion localization.
2. **Metabolic Risk Fusion:** Decision-level fusion incorporating HbA1c levels, Systolic BP, and Diabetes duration.

---

## ✨ Key System Features

- 🎯 **Disease Grading (0-4):** EfficientNet-B0 architecture trained on **APTOS 2019** dataset (No DR, Mild, Moderate, Severe, Proliferative DR).
- 🔍 **Explainable AI (XAI):** Integrated **Grad-CAM heatmaps** to highlight regions influencing predicted severity.
- 🩸 **Lesion Localization:** **U-Net** visual localization for microaneurysms, hemorrhages, and exudates.
- 🔀 **Decision Fusion Engine:** Merges ocular grades with clinical metabolic parameters for final referral recommendations (Urgent vs Standard).
- 📄 **Diagnostic Export:** Automatic PDF diagnostic report generation via `ReportLab`.
- 📊 **Domain Shift Analysis:** Benchmark testing on external **IDRID dataset** to evaluate real-world model generalization.

---

## 🏗️ Folder Structure

```text
Diabetic-Retinopathy-screening/
├── assets/                  # Performance metrics, confusion matrices & UI plots
├── docs/                    # Final project report & presentation slides (PDF)
├── notebook/                # Training, segmentation & preprocessing notebooks
├── app.py                   # Streamlit web interface engine
└── README.md                # Project documentation
