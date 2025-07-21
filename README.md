# 🛡️ Network Intrusion Detection System (NIDS)

A machine learning-powered web application that detects and classifies **network intrusions in real-time**. Built using **Flask** and trained on the **KDD Cup '99 dataset**, this system helps identify various types of network attacks and anomalies for cybersecurity monitoring.

---

## 🎯 What It Does

The system analyzes incoming network traffic and classifies it into one of the following:

- ✅ **Normal** – Safe and expected network behavior  
- 🚨 **DOS** – Denial of Service attacks  
- 🔍 **PROBE** – Port scanning and probing attempts  
- 🔓 **R2L** – Remote to Local unauthorized access  
- ⚡ **U2R** – User to Root privilege escalation attacks

---

## 🚀 Quick Start

### ✅ Prerequisites

- Python 3.x installed

### 📦 Installation

```bash
git clone https://github.com/ragulavasu/Network-Intrusion-Detection-System.git
cd Network-Intrusion-Detection-System
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

### ▶️ Run the Web App

```bash
python app.py
```

Then open your browser and visit:  
[http://localhost:5000](http://localhost:5000)

---

## 📁 Project Structure

```
Network-Intrusion-Detection-System/
├── app.py                 # Main Flask application
├── templates/
│   └── index.html         # Web interface (frontend)
├── static/                # Optional static files (CSS, images)
├── NIDS_best_model.pkl    # Pre-trained ensemble model
├── requirements.txt       # List of Python packages
└── README.md              # Project documentation
```

---

## 🔧 How to Use

1. Enter network traffic feature values in the web form.
2. Click **"Analyze Network Traffic"**.
3. View the prediction label (e.g., `Normal`, `PROBE`, etc.).
4. Use this prediction to monitor or respond to threats.

---

## 📸 Screenshots

### ✅ Prediction: Normal (Safe Traffic)
![Normal Prediction]![Alt Text](Results\Screenshot 2025-07-21 153608.png)

### 🚨 Prediction: PROBE (Threat Detected)
![Probe Prediction]![Alt Text](Results\Screenshot 2025-07-21 153033.png)


---

## 📊 Model Details

- Model File: `NIDS_best_model.pkl`
- Frameworks: `scikit-learn`, `xgboost`
- Training Dataset: [KDD Cup 1999 Dataset](http://kdd.ics.uci.edu/databases/kddcup99/kddcup99.html)
- Type: Ensemble Voting Classifier with Logistic Regression, Random Forest, Gradient Boosting, and XGBoost

---


## 📄 License

Distributed under the **MIT License**. See `LICENSE` for details.

---

## 📬 Contact

**Ragula Vasu**  
GitHub: [@ragulavasu](https://github.com/ragulavasu)  
Email: *vasuragula436@gmail.com*

---

## 🙏 Acknowledgements

- [KDD Cup 1999 Dataset](http://kdd.ics.uci.edu/databases/kddcup99/kddcup99.html)
- [Scikit-learn Documentation](https://scikit-learn.org/stable/)
- [XGBoost](https://xgboost.readthedocs.io/)
- [Flask](https://flask.palletsprojects.com/)
