# 🚀 AI-PhishingShield: Real-Time AI-Powered Phishing Detector 🛡️

[![Hackathon](https://img.shields.io/badge/Hackathon-Imagine%20Cup%202026-orange)](#)
[![Accuracy](https://img.shields.io/badge/Accuracy-95.2%25-brightgreen)](#results)
[![Live Demo](https://img.shields.io/badge/Live_Demo-blue)](https://phishingshield.vercel.app)
[![Chrome Extension](https://img.shields.io/badge/Chrome_Extension-yellow)](#quick-demo)


## 🎯 Problem Statement

Phishing attacks cause **₹10,000+ Crore annual losses in India**, especially through:
- Fake UPI requests  
- Fraud KYC links  
- Bank & government impersonation  

Traditional rule-based filters **miss ~30% of attacks**, especially localized and language-based scams.

**AI-PhishingShield** is a **real-time, AI-powered phishing detection system** that analyzes URLs, emails, and SMS messages to warn users instantly.


## 👥 Target Users & Impact

- 🎯 **Primary Users**: Indian internet users vulnerable to UPI, banking & KYC fraud  
- 🏦 **Secondary Users**: Banks, fintech platforms, email/SMS providers  
- 📉 **Impact**: Early detection can reduce phishing-related losses by **30–40%**  
- 🌍 **Scalability**: Language-agnostic architecture enables global expansion  

---

## ✨ Key Features

- 🔍 **Multi-Channel Detection**  
  Detects phishing in **URLs, emails, and SMS** (Hindi & English)

- 🤖 **AI-Based Analysis**  
  XGBoost classifier + NLP-based text analysis

- ⚡ **Real-Time Protection**  
  Chrome extension & REST API (response < 200ms)

- 📊 **Risk Scoring System**  
  Low / Medium / High risk with explainable reasons

- 🇮🇳 **India-Focused Threats**  
  Detects fake government schemes, bank alerts & UPI fraud patterns
  

## 🏗️ Tech Stack

| Component | Technology |
|---------|------------|
| Backend | Python, Flask, XGBoost |
| Frontend | React, HTML (Chrome Extension) |
| NLP | Scikit-learn |
| Dataset | PhishTank + UCI ML Repository |
| Deployment | Vercel, Replit |


## 📊 Model Training & Evaluation

- 📦 **Dataset Size**: 10,000 phishing & legitimate samples  
- 🔀 **Train/Test Split**: 80% / 20%  
- 🌐 **Languages**: English + Hindi text included  
- 🎯 **Optimization Goal**: Minimize **false negatives** (missed phishing)


## 📈 Results

- ✅ **Accuracy**: 95.2%  
- ✅ **F1-Score**: 0.94  

**Confusion Matrix:**

![Confusion Matrix](results/confusion_matrix.png)

> Model evaluated on unseen test data to avoid overfitting.


## 🚀 Quick Demo

### Chrome Extension
1. Load extension in Chrome (`Load Unpacked`)
2. Visit a phishing URL  
3. Instant alert: **“HIGH RISK – Fake Bank Login Detected”**

### API Test
```bash
curl http://api.phishingshield.com/predict?url=phishy-example.com
