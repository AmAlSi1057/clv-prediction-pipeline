# End-to-End Customer Lifetime Value (CLV) Prediction Pipeline

![Project Status](https://img.shields.io/badge/status-in%20progress-yellow)
![License](https://img.shields.io/badge/license-MIT-blue)

An open-source research project to architect and build a professional-grade, end-to-end data pipeline for predicting Customer Lifetime Value (CLV) on a real-world e-commerce dataset.

---

## 1. Business Problem & Project Goal

In e-commerce, identifying high-value customers early is critical for targeted marketing, retention efforts, and maximizing profitability. This project aims to solve this by building a system that predicts the future revenue a customer will generate based on their initial characteristics and purchasing behavior.

The primary goal is to create a robust, reproducible, and well-documented pipeline that mirrors a professional data science workflow, from raw data engineering to model deployment.

## 2. Tech Stack & Architecture

This project utilizes a modern, industry-standard data stack to ensure scalability and reproducibility.

**Tech Stack:**
* **Language:** Python 3.11
* **Data Storage:** PostgreSQL (managed with Docker)
* **Data Transformation:** dbt (Data Build Tool)
* **ML & Data Manipulation:** Pandas, Scikit-learn, XGBoost
* **Web App / Demo:** Streamlit
* **Environment & Packaging:** Poetry, Git

**Project Architecture:**

`Raw Data (CSVs) -> [PostgreSQL in Docker] -> [dbt Transformation] -> Clean Analytical Table -> [Python ML Pipeline (Train/Predict)] -> Trained Model (.pkl) -> [Streamlit Demo App]`

## 3. Current Status

⚠️ **Project in Progress: Phase 1 - Data Engineering & Transformation.**

Currently focused on building the foundational data models in `dbt` to transform the raw, multi-table Olist dataset into a clean, single analytical base table ready for machine learning.

## 4. Project Roadmap

- [x] **Phase 0: Setup & Architecture**
    - [x] Define business problem and project scope.
    - [x] Initialize GitHub repository and project structure.
    - [x] Set up Dockerized PostgreSQL environment.
    - [x] Initialize dbt project.
- [ ] **Phase 1: Data Engineering & Transformation (In Progress)**
    - [ ] Load raw data into PostgreSQL.
    - [ ] Build staging models in dbt to clean data.
    - [ ] Build a final `marts` model in dbt to create the analytical base table with engineered features (RFM, etc.).
- [ ] **Phase 2: Modeling & Experimentation**
    - [ ] Conduct Exploratory Data Analysis (EDA).
    - [ ] Develop a Scikit-learn preprocessing pipeline.
    - [ ] Train baseline and XGBoost models.
    - [ ] Evaluate model performance and analyze feature importance.
- [ ] **Phase 3: Packaging & Automation**
    - [ ] Refactor notebook code into a reusable, installable Python package.
    - [ ] Create a Command-Line Interface (CLI) for running predictions.
- [ ] **Phase 4: Deployment & Presentation**
    - [ ] Build an interactive Streamlit web application to demonstrate the model.
    - [ ] Deploy the Streamlit app to a public cloud service.
- [ ] **Phase 5: Documentation & Promotion**
    - [ ] Finalize this README with setup instructions and results.
    - [ ] Write a detailed blog post explaining the project lifecycle and findings.

## 5. Getting Started

*(This section will be filled out later with instructions on how to set up the environment and run the project.)*

## 6. License

This project is licensed under the MIT License. See the `LICENSE` file for details.
