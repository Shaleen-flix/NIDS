
# 🛡️ Network Intrusion Detection System (NIDS) via Machine Learning

**Project:** Machine Learning‑based NIDS deployed using IBM Cloud Lite (watsonx.ai Studio & Runtime)  
**Author:** Shaleen Bapna — Computer Science & Engineering (Cybersecurity)  

---

## 🔍 Overview

This repository contains a streamlined ML pipeline for detecting network intrusions (binary classification: *normal* vs *anomaly*) using the NSL-KDD dataset. The solution is built entirely in IBM Cloud Lite using **watsonx.ai Studio** for model development and **watsonx.ai Runtime** for deployment.

---

## 🧩 Problem Statement

Network security systems need intelligent, data-driven methods to identify attacks like DoS, Probe, R2L, and U2R. This project aims to automate detection of such threats using supervised learning, enabling early alerts and robust defense mechanisms.

---

## 🛠️ Solution Architecture

1. **Data Processing** — Encoding categorical features, scaling numerical fields, handling class imbalance  
2. **Modeling** — Training a **Random Forest Classifier** to distinguish *normal* traffic from *anomalies*  
3. **Evaluation** — Use accuracy, recall, precision, and confusion matrix to validate performance  
4. **Deployment** — Saving the trained model and exposing it via **watsonx.ai Runtime API** for inference

---

## 🧰 Technology Stack

| Layer | Technology |
|-------|------------|
| Development | Python 3.11, Jupyter Notebook (watsonx.ai Studio) |
| Storage | IBM Cloud Object Storage (Lite) |
| Modeling | scikit-learn, pandas, seaborn, matplotlib |
| Deployment | watsonx.ai Runtime (Cloud API endpoint) |

---

## 📥 Dataset

- Source: Kaggle – [NSL‑KDD dataset](https://www.kaggle.com/datasets/sampadab17/network-intrusion-detection)  
- Files:
  - `Train_data.csv` — labeled training set  
  - `Test_data.csv` — unlabeled test set for predictions  

---

## 📊 Model Training & Results

- **Train/Validation split:** 80/20  
- **Model:** Random Forest (n_estimators=100)  
- **Validation accuracy:** 100%  
- **F1‑score:** 1.00 for both classes  
- **Confusion Matrix:**
  ```
  [[2358   7]
   [   4 2670]]
  ```

---

## 📦 Repository Structure

```
NIDS‑ML‑IBMCloud/
│
├── NIDS_notebook.ipynb       # Complete ML workflow
├── Train_data.csv            # Training dataset (Kaggle NSL‑KDD)
├── Test_data.csv             # Test dataset
├── requirements.txt          # Pip install list
├── README.md                 # Project documentation (this file)
├── project_report.pptx       # Optional project presentation
├── project_report.pdf        # Optional project presentation
└── LICENSE                   # MIT License 
```

---

## 🚀 Getting Started

1. Clone the repository:  
   ```bash
   git clone https://github.com/<your-username>/NIDS‑ML‑IBMCloud.git
   cd NIDS‑ML‑IBMCloud
   ```
2. Install dependencies:  
   ```bash
   pip install -r requirements.txt
   ```
3. Open the notebook (`NIDS_notebook.ipynb`) locally or upload to your own IBM watsonx.ai Studio if replicating.
4. Run all cells to preprocess, train, predict, and save outputs.

---

## 🔭 Future Improvements

- **Multiclass classification** (DoS, Probe, R2L, U2R)
- **Real-time network stream ingestion** with Kafka or similar
- **Extended modeling**: XGBoost, neural networks, ensemble methods
- **Dashboard integration**: Node-RED, Flask, or similar
- **Edge deployments** on IoT or mobile devices for live intrusion detection

---

## 🙌 Acknowledgments

- IBM Cloud Lite for offering free development & deployment services  
- Kaggle community for NSL‑KDD dataset  
- Open-source libraries: scikit-learn, pandas, seaborn, matplotlib  

---

## 📝 License

MIT License – feel free to use, modify, and distribute the project under its terms.

---

## 📬 Contact

**Shaleen Bapna**  
Email: shaleenbapna13@gmail.com  
GitHub: [shaleenbapna](https://github.com/Shaleen-flix)  
LinkedIn: www.linkedin.com/in/shaleen-bapna
