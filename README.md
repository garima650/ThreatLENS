# ThreatLENS

## AI-Powered Scam & Fraud Intelligence Platform

ThreatLENS is an AI-powered scam and fraud intelligence platform designed to detect suspicious messages, analyze potentially malicious URLs, identify fraud patterns, and provide an interactive security dashboard for understanding emerging threats.

It combines **TF-IDF + Logistic Regression**, **DistilBERT-based text classification**, and **URL analysis** to provide a multi-layered approach to scam detection.

## Features

- AI-powered scam and fraud detection
- TF-IDF + Logistic Regression classification
- DistilBERT transformer-based contextual analysis
- Hybrid decision system
- Suspicious URL analysis
- Risk classification: LOW, MEDIUM, HIGH
- SCAM / LEGITIMATE / REVIEW predictions
- Interactive security dashboard
- Scanner Ring for threat distribution
- Live Security Activity monitoring
- Fraud Pattern Movement visualization
- Fraud category intelligence
- Scan history
- Message Analyzer
- URL Analyzer
- Dark security-focused interface

## Detection System

ThreatLENS uses two independent machine learning models to analyze messages.

```text
                    MESSAGE
                       |
          +------------+------------+
          |                         |
          v                         v
   TF-IDF + Logistic          DistilBERT
      Regression              Transformer
          |                         |
          +------------+------------+
                       |
                       v
                 DECISION LAYER
                       |
          +------------+------------+
          |            |            |
          v            v            v
        SCAM       LEGITIMATE     REVIEW
```

## The ThreatLENS dashboard acts as a centralized security command center.
It provides:
Scanner Ring
A concentric visualization showing:
- Legitimate scans
- Review cases
- Scam detections
Live Security Activity
Displays security-analysis activity over time and helps visualize changes in scan volume.
Fraud Pattern Movement
Tracks fraud activity across different categories such as:
- Bank Fraud
- Loan Fraud
- Police / Digital Arrest
- OTP / Phishing
Threat Categories
Current categories include:
- Bank Fraud
- Loan Fraud
- Police / Digital Arrest
- Courier / Parcel
- OTP / Phishing
- Lottery / Prize
Scan History
Previous analyses are displayed with their prediction, risk level, message, and timestamp.
Machine Learning
The project uses a combined dataset containing approximately 39,700 messages from multiple scam and spam datasets.
The training data includes sources such as:
- ICFD-31k
- SMS Spam Collection
- Scam/Spam India
- Indian Cyber Scam Hinglish Dataset
- Financial Scams Detection Dataset

## Data processing pipelines:
```text
Raw Datasets
     ↓
Data Cleaning
     ↓
Deduplication
     ↓
Label Processing
     ↓
Dataset Combination
     ↓
Train/Test Split
     ↓
Model Training
     ↓
Evaluation
     ↓
Saved Models

## Technology Stack
Frontend
- Streamlit
- HTML
- CSS
- SVG
Backend
- FastAPI
- Uvicorn
- Pydantic
Machine Learning
- Python
- Scikit-learn
- TF-IDF
- Logistic Regression
- Transformers
- DistilBERT
- PyTorch
- Joblib
Data Processing
- Pandas
- NumPy

ThreatLENS/
│
├── backend/
│   ├── main.py
│   ├── schemas.py
│   └── services/
│       ├── scam_detector.py
│       ├── transformer_detector.py
│       └── url_analyzer.py
│
├── dataset/
│
├── models/
│   ├── scam_model.pkl
│   ├── tfidf_vectorizer.pkl
│   └── scam_transformer/
│
├── training/
│
├── frontend/
│   ├── app.py
│   └── pages/
│       ├── login.py
│       └── dashboard.py
│
├── requirements.txt
└── README.md
```
## Future Improvements
- Screenshot-based scam detection
- OCR integration
- Multilingual scam detection
- Advanced URL intelligence
- AI-powered scam investigation
- Trusted-source verification
- Scam-chain detection
- Personalized security recommendations
- Persistent database-backed history
- Improved transformer training

## Disclaimer
ThreatLENS is an experimental security analysis platform. Machine learning predictions should be treated as security signals rather than guaranteed verdicts.
Users should independently verify important security information through official channels and should never share passwords, OTPs, recovery codes, or other sensitive credentials based solely on an automated prediction.
License
This project is intended for educational, research, and development purposes.

ThreatLENS
See the threat. Understand the pattern. Stay protected.
