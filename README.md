FinSentinel 🚨
AI-Powered Real-Time Fraud Detection Backend System

FinSentinel is an intelligent fraud detection backend system designed to analyze financial transactions in real time using Machine Learning, Rule-Based Analysis, and Risk Scoring techniques.

The system evaluates every incoming transaction before completion and classifies it as:

✅ Safe
⚠️ Suspicious
🚫 Fraud

Based on the risk score, FinSentinel can automatically:

Approve transactions
Trigger OTP verification
Block fraudulent transactions
📌 Features
🔹 Real-Time Fraud Detection

Analyzes transactions instantly before completion.

🔹 Hybrid Detection Engine

Combines:

Machine Learning
Rule-Based Fraud Analysis

for better accuracy and explainability.

🔹 AI Risk Scoring

Generates a fraud risk score from:

0 – 100

using:

XGBoost predictions
Fraud rules
Behavioral signals
🔹 Smart Decision System
Risk Level	Decision
Safe	Approved
Suspicious	OTP Required
Fraud	Blocked
🔹 Rule-Based Fraud Detection

Implemented fraud rules:

High Amount Detection
Amount Anomaly Detection
New Device Detection
Unusual Location Detection
Odd Hour Transactions
Rapid Transaction Velocity
Foreign Currency Detection
🔹 Analytics Dashboard APIs

Provides APIs for:

Fraud statistics
Risk distribution
Hourly fraud analysis
Recent transactions
Top flagged fraud rules
🏗️ System Architecture
User Transaction
       ↓
Flask API Gateway
       ↓
Risk Engine + Rule Engine
       ↓
XGBoost Fraud Model
       ↓
Risk Scoring System
       ↓
Decision Engine
       ↓
Database Storage
       ↓
Dashboard APIs
🧠 Machine Learning Pipeline

The ML pipeline performs:

Data preprocessing
Feature scaling
Class balancing using SMOTE
XGBoost training
Fraud probability prediction

Dataset used:

Kaggle Credit Card Fraud Detection Dataset
📊 Model Performance
Metric	Score
Accuracy	99.84%
Precision	52.8%
Recall	86.7%
F1 Score	65.6%
AUC-ROC	97.97%
🛠️ Tech Stack
Backend
Flask
Flask-CORS
Flask-SQLAlchemy
Database
SQLite (Current)
PostgreSQL (Planned)
Machine Learning
Scikit-learn
XGBoost
imbalanced-learn
pandas
numpy
Utilities
joblib
python-dotenv
Streaming & Future Enhancements
Apache Kafka
SHAP Explainability
Deep Learning Models
Graph Neural Networks (Planned)
📂 Project Structure
FinSentinel/
│
├── database/
├── model/
├── routes/
├── services/
├── streaming/
├── tests/
├── training/
├── utils/
│
├── app.py
├── config.py
├── requirements.txt
├── docker-compose.yml
└── Dockerfile
🔌 API Endpoints
Transaction APIs
Analyze Transaction
POST /api/transaction/analyze
Transaction History
GET /api/transaction/history
Get Transaction Details
GET /api/transaction/<transaction_id>
Dashboard APIs
Fraud Statistics
GET /api/dashboard/stats
Recent Transactions
GET /api/dashboard/recent
Risk Distribution
GET /api/dashboard/risk-distribution
Hourly Fraud Trends
GET /api/dashboard/hourly-fraud
⚙️ Installation
Clone Repository
git clone https://github.com/Rhys3009/FinSentinel.git
Navigate to Backend
cd finsentinel-backend
Create Virtual Environment
python -m venv venv
Activate Environment
Windows
venv\Scripts\activate
Linux / Mac
source venv/bin/activate
Install Dependencies
pip install -r requirements.txt
Train ML Model
python model/train_model.py
Run Backend
python app.py
🚀 Future Enhancements
PostgreSQL Integration
Kafka Streaming Architecture
SHAP Explainability Layer
Neural Network Fraud Models
Graph Neural Networks (GNN)
Real-Time Alerts & Notifications
Advanced Analytics Dashboard
Docker Deployment
Kubernetes Scaling
👨‍💻 Author
Rhys Nunes

Computer Science Student | Backend & AI Enthusiast

GitHub:
Rhys3009 GitHub Profile

⭐ Project Status

✅ Active Development
🚀 Production-Oriented Fraud Detection Architecture
🔐 FinTech Security Focused
