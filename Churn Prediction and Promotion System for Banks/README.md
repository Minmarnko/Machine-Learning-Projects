
# 🏦 Churn Prediction and Promotion System for Banks

This project presents a machine learning-based system that integrates **supervised** and **unsupervised** learning methods to enhance customer retention and personalized promotions in the banking sector. The application predicts customer churn using classification models and segments customers using clustering techniques for targeted marketing strategies. The solution is production-ready, deployed using Docker and hosted on AWS EC2.

## 📊 Project Overview

**Objective:**  
To predict customer churn and provide intelligent promotional strategies using data-driven methods.

**Key Features:**
- Supervised learning (Random Forest, Logistic Regression, Gradient Boosting)
- Unsupervised learning (K-Means Clustering)
- SMOTE for class balancing
- Feature engineering and importance analysis
- CI/CD deployment using Docker, GitHub Actions, and AWS EC2
- User-friendly web application for real-time churn prediction and customer segmentation

---

## 🔍 Data Pipeline & Modeling

### 🔧 Supervised Learning (Churn Prediction)
- **Preprocessing:** Null value handling, label encoding, MinMax scaling
- **Balancing:** SMOTE to handle class imbalance
- **Models:** Logistic Regression, Random Forest, Gradient Boosting
- **Best Model:** Random Forest (Accuracy ≈ 84%)
- **Evaluation:** Classification report, confusion matrix, feature importance

### 🔍 Unsupervised Learning (Customer Segmentation)
- **Features Used:** Age, job, marital status, education, balance, housing loan, personal loan, default status, deposit
- **Technique:** K-Means Clustering
- **Best K:** 4 (selected using Elbow Method & Silhouette Score)
- **Output:** Cluster-based promotional strategies

---

## 🚀 Deployment Architecture

### 🔧 Tools Used:
- Docker
- GitHub Actions (CI/CD)
- AWS EC2
- Streamlit for web application

### 📦 Deployment Steps:
1. Build and push Docker image to Docker Hub
2. Use GitHub Actions to pull and deploy the image to AWS EC2
3. Application served via `http://34.209.204.206:8080/`

---

## 🌐 Web Application

- **Churn Prediction Page:** Input customer features to predict likelihood of churn
- **Cluster Assignment Page:** Segment new customer into one of 4 predefined clusters
- **Tailored Promotions:** Display recommended offers based on the cluster

---

## 📁 Repository Structure

\`\`\`bash
ML-Group4/
├── app/                  # Streamlit web app
├── model/                # Trained models & clustering pipeline
├── data/                 # Sample data used for training/testing
├── Dockerfile            # For containerization
├── requirements.txt      # Python dependencies
├── deploy.yml            # GitHub Actions workflow
├── README.md             # Project overview
└── report/               # Final project report (PDF, figures)
\`\`\`

---

## 🔗 Useful Links

- 🐳 **DockerHub:** [Group4 Deployment](https://hub.docker.com/repository/docker/sonakul/group4-deployment/)
- 🌐 **Live Demo:** [Web Application](http://34.209.204.206:8080/)

---

## 📚 References

This project references insights from McKinsey, Accenture, Gartner, and other leading financial and data analytics publications. Full citations can be found in the [report](./report/Group4%20Final%20report.pdf).
