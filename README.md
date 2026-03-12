🔐 Network Security Threat Detection System

A Machine Learning based system designed to detect malicious or suspicious network activity using multiple classification models.
The project implements a complete **ML pipeline including data preprocessing, model training, evaluation, experiment tracking, and API deployment with Swagger UI**.

# 🚀 Features

* End-to-end **machine learning pipeline for network threat detection**
* Training and comparison of multiple classification algorithms
* Automated **model selection based on evaluation metrics**
* **Experiment tracking with MLflow and DagsHub**
* REST API with **interactive Swagger UI documentation**
* Deployment-ready backend service

---

# 🧠 Machine Learning Models Used

The system trains and evaluates multiple models to determine the best performing classifier:

* Random Forest Classifier
* Gradient Boosting Classifier
* AdaBoost Classifier
* Decision Tree Classifier
* Logistic Regression

Hyperparameter tuning is applied during training to improve model performance.

The best model is selected using classification metrics such as:

* **F1 Score**
* **Precision**
* **Recall**

---

# ⚙️ ML Pipeline Architecture

The project follows a modular ML pipeline:

1. Data Ingestion
2. Data Validation
3. Data Transformation
4. Model Training
5. Model Evaluation
6. Model Saving & Versioning

MLflow is used for **experiment tracking and model logging**.

---

# 📊 Experiment Tracking

Experiments are tracked using:

* **MLflow**
* **DagsHub**

This allows logging:

* Model parameters
* Evaluation metrics
* Trained model artifacts

This helps ensure **reproducibility and experiment management**.

---

# 🌐 API Interface

The trained model is served through a REST API with **Swagger UI documentation**, allowing users to test endpoints interactively.

Example endpoints:

```
/predict
/train
/docs
```

Swagger UI provides an interactive interface for testing predictions.

---

# ☁️ Deployment

The application is currently being deployed on **Amazon Web Services using the **Amazon EC2** service.

Deployment steps include:

* Launching an EC2 instance
* Installing Python dependencies
* Running the backend API server
* Exposing the API via a public endpoint

This allows the model to be accessed remotely for real-time predictions.

---

# 🛠️ Tech Stack

**Programming Language**

* Python

**Machine Learning**

* Scikit-learn
* NumPy
* Pandas

**MLOps**

* MLflow
* DagsHub

**Backend API**

* FastAPI / Flask
* Swagger UI

**Deployment**

* AWS EC2

---

# 📂 Project Structure

```
networksecurity
│
├── components
│   ├── data_ingestion
│   ├── data_transformation
│   ├── model_trainer
│
├── utils
│   ├── ml_utils
│   ├── main_utils
│
├── pipeline
│
├── final_model
│
├── app.py
├── requirements.txt
└── README.md
```

---

# ▶️ How to Run the Project

Clone the repository:

```
git clone https://github.com/Nimisha1518/networksecurity.git
cd networksecurity
```

Create virtual environment:

```
python -m venv venv
```

Activate environment:

```
source venv/bin/activate
```

Install dependencies:

```
pip install -r requirements.txt
```

Run the application:

```
python app.py
```

Open Swagger UI:

```
http://localhost:8000/docs
```

---

# 📌 Future Improvements

* Containerization using Docker
* CI/CD integration
* Cloud deployment automation
* Real-time network packet analysis

---

# 👩‍💻 Author

**Nimisha Sharma**

GitHub:
[https://github.com/Nimisha1518](https://github.com/Nimisha1518)
