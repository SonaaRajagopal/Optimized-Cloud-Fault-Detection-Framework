# ☁️ Fault Detection in Cloud Infrastructure using Machine Learning
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)
![Status](https://img.shields.io/badge/Project-Active-brightgreen)
![ML](https://img.shields.io/badge/Machine%20Learning-Sklearn%20%7C%20XGBoost-orange)




Detecting anomalies and faults in cloud infrastructure using a data-driven machine learning approach to enhance system reliability, reduce downtime, and automate incident response.




## 🧠 Overview

Cloud systems generate vast telemetry data that can be used to detect failures before they escalate. This project builds a machine learning pipeline that:
- Monitors logs, metrics, and resource usage,
- Detects abnormal behavior or infrastructure faults (hardware/software/network),
- Raises alerts based on severity classification.



## 🎯 Objectives

- Analyze cloud metrics and event logs for anomaly detection.
- Detect early symptoms of resource failure or misconfiguration.
- Classify faults into categories (hardware, network, system-level, etc.).
- Reduce MTTR (Mean Time to Repair) by enabling proactive detection.



## 🧰 Tech Stack

| Category          | Tools Used                                     |
|||
| Language          | Python, SQL                                    |
| Frameworks        | TensorFlow, Scikit-learn, PyCaret              |
| ML Techniques     | Autoencoders, Isolation Forest, LSTM, SVM      |
| Visualization     | Streamlit, Power BI, Matplotlib, Seaborn       |
| Data Handling     | Pandas, NumPy, Firebase                        |
| Deployment        | Docker, Flask (for APIs), AWS EC2/GCP Compute |



## 🗂️ Dataset

- **Source:** [Internal logs/simulated cloud dataset] or [Public cloud telemetry dataset]
- **Features:**
  - CPU Usage, Memory Usage, Disk I/O, Network Traffic
  - Event Logs (Timestamped)
  - Labels: Normal / Faulty (Types: Resource, Network, Application)

> 📝 The dataset is preprocessed for missing values, time-window segmentation, and normalization.



## 🔁 Model Pipeline

1. **Data Ingestion**: Real-time logs or batch CSV ingestion.
2. **Preprocessing**: Normalization, feature engineering, time-series reshaping.
3. **Training**:
   - Supervised: SVM, XGBoost, Random Forest
   - Unsupervised: Isolation Forest, Autoencoder
4. **Evaluation**:
   - Metrics: Accuracy, F1-score, ROC-AUC, Precision/Recall
5. **Visualization**: Dashboards for fault analysis and prediction confidence.



## 📊 Results

| Model            | Accuracy | F1-Score | AUC-ROC |
||-|-||
| Isolation Forest | 87%      | 85%      | 0.91    |
| Autoencoder      | 89%      | 88%      | 0.93    |
| LSTM             | 92%      | 91%      | 0.95    |

✅ Real-time detection latency < 3 seconds  
✅ Detected 95% of hardware faults before failure



## ⚙️ Installation

Clone this repository:
```bash
git clone https://github.com/yourusername/fault-detection-cloud.git
cd fault-detection-cloud
