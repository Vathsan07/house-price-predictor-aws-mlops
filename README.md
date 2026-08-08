# 🏠 House Price Predictor – AWS MLOps Project

An end-to-end AWS Machine Learning project that demonstrates the complete MLOps workflow for predicting house prices using a synthetic dataset.

This project was developed as part of the **BITS Pilani – Professional Certificate in AI/ML** programme and showcases data storage, cataloging, querying, feature management, model training, and model registration using AWS services.

---

## 📌 Project Overview

The objective of this project is to build a complete machine learning pipeline capable of predicting house prices based on various property characteristics.

The project covers:

- Synthetic dataset generation
- Cloud storage using Amazon S3
- Metadata management using AWS Glue
- SQL analytics using Amazon Athena
- Feature management using SageMaker Feature Store
- Machine learning model training using Scikit-Learn
- Model packaging and registration using SageMaker Model Registry

---

## 🏡 Business Problem

Real estate companies need accurate and consistent house price predictions based on property features.

This project demonstrates how an end-to-end AWS MLOps pipeline can be used to manage data, train machine learning models, and register model versions while maintaining reproducibility and governance.

---

## 🛠️ Technologies Used

### Programming

- Python 3.x
- Jupyter Notebook
- NumPy
- Pandas
- Scikit-Learn
- boto3

### AWS Services

- Amazon S3
- AWS Glue Data Catalog
- Amazon Athena
- Amazon SageMaker Feature Store
- Amazon SageMaker Model Registry

---

## 📂 Repository Structure

```
house-price-predictor-aws-mlops/
│
├── notebooks/
│   └── HousePricePredictor.ipynb
│
├── dataset/
│   └── houses.csv
│
├── report/
│   ├── Assignment_Report.pdf
│   └── Assignment_Report.docx
│
├── screenshots/
│
├── README.md
├── LICENSE
└── .gitignore
```

---

## 🔄 Project Workflow

```
Generate Synthetic Dataset
          │
          ▼
Upload Dataset to Amazon S3
          │
          ▼
Create Glue Database & External Table
          │
          ▼
Query Data using Amazon Athena
          │
          ▼
Create SageMaker Feature Store
          │
          ▼
Ingest Features
          │
          ▼
Train Random Forest Model
          │
          ▼
Package Model (model.tar.gz)
          │
          ▼
Upload Model to Amazon S3
          │
          ▼
Register Model in SageMaker Model Registry
```

---

## 📊 Dataset

The project uses a synthetic dataset containing **500 residential house records**.

### Features

- size_sqft
- bedrooms
- age_years
- distance_km
- has_garage

### Target Variable

- price_usd

---

## 🤖 Machine Learning Model

**Algorithm**

Random Forest Regressor

### Training Configuration

| Parameter | Value |
|-----------|------:|
| Number of Trees | 100 |
| Train/Test Split | 80/20 |
| Random State | 42 |

---

## 📈 Model Performance

| Metric | Value |
|---------|-------:|
| Mean Absolute Error (MAE) | 26,019.20 |
| Root Mean Squared Error (RMSE) | 33,920.81 |
| R² Score | 0.9131 |

### Feature Importance

| Rank | Feature | Importance |
|------|----------|-----------:|
| 1 | size_sqft | 0.638687 |
| 2 | distance_km | 0.272966 |
| 3 | age_years | 0.043274 |
| 4 | bedrooms | 0.036395 |
| 5 | has_garage | 0.008677 |

---

## 📸 Project Screenshots

The repository includes screenshots demonstrating:

- Dataset Generation
- Amazon S3 Bucket Structure
- AWS Glue Data Catalog
- Amazon Athena Query
- SageMaker Feature Store
- Model Packaging
- SageMaker Model Registry
- Model Evaluation

---

## 🚀 How to Run

1. Clone the repository.

```bash
git clone https://github.com/<your-username>/house-price-predictor-aws-mlops.git
```

2. Install the required dependencies.

```bash
pip install boto3 pandas numpy scikit-learn jupyter
```

3. Configure AWS CLI.

```bash
aws configure
```

4. Open the notebook.

```bash
jupyter notebook
```

5. Execute the notebook sequentially.

---

## 🎯 Project Outcomes

Successfully implemented an end-to-end AWS Machine Learning workflow covering:

- Data Generation
- Amazon S3 Storage
- AWS Glue Data Catalog
- Amazon Athena SQL Queries
- SageMaker Feature Store
- Random Forest Model Training
- Model Packaging
- SageMaker Model Registry

---

## 🔮 Future Improvements

Possible enhancements include:

- Deploy the trained model as a SageMaker endpoint.
- Automate the pipeline using AWS Step Functions.
- Integrate CI/CD for model deployment.
- Add model monitoring and drift detection.
- Replace the synthetic dataset with real-world housing data.

---

## 👨‍💻 Author

**Shrivathsan K M**

BITS Pilani – Professional Certificate in AI/ML

---

## ⭐ Acknowledgement

This project was developed as part of the **AWS Machine Learning Basics Lab** under the **BITS Pilani Professional Certificate in AI/ML** programme.
