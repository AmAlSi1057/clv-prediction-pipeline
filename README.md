# End-to-End Customer Lifetime Value (CLV) Prediction Pipeline

![Project Status](https://img.shields.io/badge/status-in%20progress-yellow)
![License](https://img.shields.io/badge/license-MIT-blue)

An open-source project to build a professional-grade, cloud-native, end-to-end data pipeline for predicting Customer Lifetime Value (CLV) in a realistic 2-4 week sprint.

---

## 1. Business Problem & Project Goal

In e-commerce, identifying high-value customers early is critical for targeted marketing and maximizing profitability. This project builds a system to predict future customer revenue based on initial purchasing behavior. The goal is to create a robust, end-to-end pipeline that mirrors a modern, agile data science workflow, resulting in a deployable asset.

## 2. Tech Stack & Architecture

This project utilizes a modern, industry-standard, cloud-native data stack.

* **Cloud Platform:** Google Cloud Platform (GCP)
* **Data Warehouse:** Google BigQuery
* **Data Transformation:** dbt (Data Build Tool)
* **ML & Data Manipulation:** Python, Pandas, Scikit-learn, XGBoost
* **API & Deployment:** FastAPI, Docker
* **Web App / Demo:** Streamlit
* **Code Management:** Git, GitHub

**Project Architecture:**

`Raw Data (CSVs) -> [Google BigQuery] -> [dbt Transformation] -> Clean Analytical Table -> [Python ML Pipeline] -> Trained Model (.pkl) -> [FastAPI in Docker] -> [Streamlit App]`

## 3. Current Status

✅ **Phase 0: Project Setup & Planning Complete.**
▶️ **Phase 1: Week 1 - Core Pipeline (MVP) in Progress.**

## 4. Project Roadmap (2-4 Week Sprint)

### **Week 1: Core Pipeline (MVP)**
- [ ] **Setup & Data Loading:**
    - [ ] Set up Google Cloud Platform (GCP) project and BigQuery dataset.
    - [ ] Load Olist dataset into BigQuery.
    - [ ] Initialize dbt project and connect to BigQuery.
- [ ] **Basic Data Transformation:**
    - [ ] Build simple dbt `staging` models to clean data.
    - [ ] Create one analytical `mart` table with foundational features (e.g., RFM).
    - [ ] Implement basic dbt tests for data quality checks.
- [ ] **Simple Model:**
    - [ ] Conduct basic EDA in a Jupyter Notebook.
    - [ ] Train a baseline XGBoost model with cross-validation.
    - [ ] Save the trained model artifact and document the initial approach.

### **Week 2: Make It Production-Ready**
- [ ] **API Development:**
    - [ ] Build a simple FastAPI with a `/predict` endpoint.
    - [ ] Implement basic input validation with Pydantic.
    - [ ] Containerize the API using Docker.
- [ ] **Basic Frontend:**
    - [ ] Build a Streamlit application with file upload and prediction display.
    - [ ] Add simple visualizations of the results and feature importances.
- [ ] **Documentation & Polish:**
    - [ ] Update this README with setup instructions and results.
    - [ ] Deploy the Streamlit app to a public service (e.g., Streamlit Community Cloud).

### **Weeks 3-4: Enhance & Differentiate (Optional Stretch Goals)**
- [ ] Add one advanced feature (e.g., SHAP explanations for model interpretability).
- [ ] Write a detailed blog post on Medium explaining the project and findings.
- [ ] Implement basic CI/CD with GitHub Actions to automate testing or deployment.

## 5. Getting Started

*(This section will be filled out with instructions on how to set up the environment, configure GCP credentials, and run the project.)*

## 6. License

This project is licensed under the MIT License. See the `LICENSE` file for details.
