# 🎓 Student Performance Prediction – End-to-End ML Production Pipeline

An **end-to-end machine learning project** that predicts student academic performance using multiple regression models, advanced **EDA**, **hyperparameter tuning**, and a **production-ready ML pipeline** deployed on cloud infrastructure.

The project demonstrates a **complete industry ML workflow** from raw data analysis to **cloud deployment using containerized infrastructure**.

---

# 🚀 Project Highlights

✔ Comprehensive **Exploratory Data Analysis (EDA)**<br>
✔ **7 Machine Learning Algorithms Compared**<br>
✔ **Hyperparameter Tuning for Model Optimization**<br>
✔ **Modular Production-Level ML Pipeline**<br>
✔ **Flask Web Application for Predictions**<br>
✔ **AWS Elastic Beanstalk Deployment**<br>
✔ **Docker Containerization**<br>
✔ **Azure Container Deployment**<br>
✔ **AWS EC2 + ECR Container Registry Integration**<br>

---

# 📊 Problem Statement

Predict student academic performance based on demographic, social, and academic attributes.
Such models can help **educational institutions identify students needing support early**.

Target Variable:

```
Math Score
```

---

# 📂 Project Structure

```
STUDENT-PERFORM/
│
├── artifacts/                     # Trained models & pipeline artifacts
│
├── logs/                          # Application logs
│
├── notebook/                      # Research & experimentation
│   ├── data/
│   ├── 1.EDA STUDENT PERFORMANCE.ipynb
│   └── 2.MODEL TRAINING.ipynb
│
├── src/
│   │
│   ├── components/                # Core ML pipeline components
│   │   ├── data_ingestion.py
│   │   ├── data_transformation.py
│   │   └── model_trainer.py
│   │
│   ├── pipeline/
│   │   ├── train_pipeline.py
│   │   └── predict_pipeline.py
│   │
│   ├── exception.py
│   ├── logger.py
│   └── utils.py
│
├── templates/
│   ├── home.html
│   └── index.html
│
├── application.py                 # Flask application
├── requirements.txt
├── setup.py
└── README.md
```

---

# 📈 Exploratory Data Analysis

Extensive **EDA** was conducted to understand the dataset:

Key insights explored:

• Feature distributions
• Correlation analysis
• Outlier detection
• Impact of demographic variables
• Feature relationships with student scores
• Visualization of performance trends

Libraries used:

* Pandas
* NumPy
* Matplotlib
* Seaborn

---

# 🤖 Machine Learning Models Used

The following regression algorithms were trained and evaluated:

```
Random Forest Regressor
Decision Tree Regressor
Gradient Boosting Regressor
Linear Regression
XGBoost Regressor
CatBoost Regressor
AdaBoost Regressor
```

Each model was evaluated and compared using performance metrics.

---

# ⚙️ Hyperparameter Tuning

Hyperparameter tuning was applied to improve model performance using **Grid Search / cross-validation techniques**.

Optimized parameters include:

* Tree depth
* Number of estimators
* Learning rate
* Regularization parameters
* Feature sampling strategies

This ensures the **best performing model is selected automatically**.

---

# 📊 Model Evaluation Metrics

Models were evaluated using:

* **R² Score**
* **Mean Absolute Error (MAE)**
* **Mean Squared Error (MSE)**

The pipeline selects the **best performing model** based on evaluation results.

---

# 🧠 ML Pipeline Architecture

The project implements a modular **production ML pipeline**:

### 1️⃣ Data Ingestion

* Reads dataset
* Splits train/test data
* Saves artifacts

### 2️⃣ Data Transformation

* Missing value handling
* Encoding categorical features
* Feature scaling
* Pipeline creation using `sklearn`

### 3️⃣ Model Training

* Train multiple models
* Hyperparameter tuning
* Model evaluation
* Best model selection

### 4️⃣ Prediction Pipeline

* Load trained model
* Apply preprocessing pipeline
* Generate predictions

---

# 🌐 Web Application

A simple **Flask web interface** allows users to input student information and obtain predicted scores.

Users can:

• Enter student features
• Submit the form
• Receive predicted academic performance

---

# ☁️ Cloud Deployment

The project is deployed using **multiple cloud environments**, simulating real production workflows.

### AWS Deployment

* **AWS Elastic Beanstalk** for application hosting
* **EC2 instances** for runtime environment
* **Amazon ECR** used as container registry

Workflow:

```
Docker Image → Push to ECR → Deploy on EC2 → Elastic Beanstalk Hosting
```

---

### Azure Deployment

Containerized application deployed using:

* **Azure Container Services**
* **Docker images**
* Scalable container environment

---

# 🐳 Containerization

The application is containerized using **Docker** to ensure portability across environments.

Benefits:

* Consistent environment
* Easy deployment
* Cloud compatibility
* Reproducibility

---

# 🛠 Tech Stack

### Programming

Python

### Machine Learning

* Scikit-Learn
* XGBoost
* CatBoost

### Data Analysis

* Pandas
* NumPy

### Visualization

* Matplotlib
* Seaborn

### Backend

Flask

### Cloud & DevOps

* AWS Elastic Beanstalk
* AWS EC2
* Amazon ECR
* Azure Container Deployment
* Docker

---

# 🖥 Running Locally

### Clone Repository

```
git clone https://github.com/yourusername/student-performance-ml-project.git
```

```
cd student-performance-ml-project
```

---

### Create Virtual Environment

```
python -m venv venv
```

Activate:

Windows

```
venv\Scripts\activate
```

Mac/Linux

```
source venv/bin/activate
```

---

### Install Dependencies

```
pip install -r requirements.txt
```

---

### Run Application

```
python application.py
```

Application runs on:

```
http://localhost:5000
```

---

# 📦 Artifacts Generated

The `artifacts/` folder contains:

• Trained ML model<br>
• Preprocessing pipeline<br>
• Train/Test datasets<br>
• Serialized objects for inference<br>

This enables **reproducible predictions and production deployment**.

---

# 🧾 Logging & Exception Handling

The system includes structured:

• Logging<br>
• Custom exception handling<br>
• Debug-friendly error tracking<br>

Logs are stored inside:

```
logs/
```

---

# 🎯 Future Improvements

Possible enhancements:

* CI/CD automation
* Model monitoring
* Feature store integration
* FastAPI REST API
* Kubernetes deployment
* Real-time prediction API

---

# 👨‍💻 Author

**Sagar Rai**

Machine Learning & AI Engineer (Aspiring)  
Focused on building production-ready ML systems, data-driven applications, and cloud-deployed AI solutions.

🔗 GitHub: https://github.com/sagarraii 
🔗 LinkedIn: https://www.linkedin.com/in/mr-raiii/
---

# ⭐ Support

If you find this project useful:

⭐ Star the repository
🔁 Share it with others
