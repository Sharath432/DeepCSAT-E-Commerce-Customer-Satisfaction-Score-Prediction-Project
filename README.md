# 🛒 DeepCSAT - E-Commerce Customer Satisfaction Score Prediction using Deep Learning (ANN)

# 📌 Project Overview

Customer satisfaction plays a crucial role in the success of any e-commerce business. Understanding customer experiences and predicting their satisfaction levels enables organizations to improve service quality, reduce customer churn, and optimize operational efficiency.

This project develops a **Deep Learning based Artificial Neural Network (ANN)** to predict **Customer Satisfaction (CSAT) Scores** using customer support interaction data from an e-commerce platform.

The model learns patterns from customer interactions, product information, service response times, and agent-related features to accurately estimate customer satisfaction before manual feedback is received.

The final solution also includes a **Flask-based deployment** for real-time prediction.

---

# 🎯 Business Problem

Customer Support teams receive thousands of interactions every day.

However,

- Customer feedback is not always available.
- Dissatisfied customers may never submit surveys.
- Businesses struggle to identify poor customer experiences early.

A predictive CSAT model allows organizations to:

- Predict customer satisfaction instantly
- Detect poor customer experiences
- Improve agent performance
- Reduce customer churn
- Improve service quality

---

# 🎯 Project Objectives

- Perform comprehensive Exploratory Data Analysis (EDA)
- Clean and preprocess real-world customer support data
- Engineer meaningful features
- Build an Artificial Neural Network (ANN)
- Optimize model performance using Cross Validation and Hyperparameter Tuning
- Evaluate model performance using regression metrics
- Deploy the trained model using Flask
- Generate actionable business insights

---

# 📊 Dataset Information

The dataset contains customer support interactions collected from an e-commerce platform.

### Dataset Size

- **Rows:** 85,907
- **Columns:** 20

### Features include

- Channel Name
- Category
- Sub Category
- Customer City
- Product Category
- Item Price
- Agent Name
- Supervisor
- Manager
- Agent Shift
- Tenure Bucket
- Connected Handling Time
- Response Time
- Customer Remarks
- CSAT Score (Target Variable)

---

# 🛠 Tech Stack

### Programming

- Python

### Libraries

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- TensorFlow / Keras
- Keras Tuner

### Deployment

- Flask

### Environment

- Google Colab
- VS Code

---

# 🔄 Project Workflow

```
Business Understanding

↓

Data Collection

↓

Data Cleaning

↓

Exploratory Data Analysis

↓

Feature Engineering

↓

Data Preprocessing

↓

Train-Test Split

↓

Feature Scaling

↓

Artificial Neural Network

↓

Cross Validation

↓

Hyperparameter Tuning

↓

Model Evaluation

↓

Model Saving

↓

Flask Deployment
```

---

# 📈 Exploratory Data Analysis (EDA)

Extensive Exploratory Data Analysis was performed to understand customer behavior and identify factors affecting customer satisfaction.

The project includes more than **15 meaningful visualizations**, including:

- Distribution of CSAT Scores
- Item Price vs CSAT
- Agent Shift Analysis
- Agent Tenure Analysis
- Category-wise Satisfaction
- Sub-category Heatmaps
- Correlation Heatmap
- Pair Plot
- Histograms
- Violin Plots
- Boxplots
- Scatter Plots
- Line Charts
- Multivariate Analysis

---

# 🔍 Data Preprocessing

The following preprocessing techniques were applied:

### Missing Value Treatment

- Filled categorical values using **Unknown**
- Filled numerical values using Mean and Median

### Feature Engineering

Created new features such as

- Response Time
- Time to Survey

### Feature Selection

Removed unnecessary columns including

- Unique ID
- Order ID
- Customer Remarks
- Date Columns

### Encoding

Applied **Label Encoding** to categorical features.

### Scaling

Applied **StandardScaler** before training the ANN.

---

# 🧠 Artificial Neural Network (ANN)

The ANN architecture consists of multiple fully connected Dense layers.

### Network Architecture

Input Layer

↓

Dense Layer (128 neurons)

↓

Dropout (0.2)

↓

Dense Layer (64 neurons)

↓

Dense Layer (32 neurons)

↓

Output Layer

Activation Function:

- ReLU
- Linear Output

Optimizer:

- Adam

Loss Function:

- Mean Squared Error (MSE)

---

# ⚙ Model Optimization

The model was further improved using:

## Cross Validation

- K-Fold Cross Validation

## Hyperparameter Tuning

Implemented using

- Keras Tuner
- Hyperband Search

Parameters tuned include

- Number of neurons
- Dropout rate
- Optimizer

---

# 📉 Model Evaluation

The model performance was evaluated using

- Mean Squared Error (MSE)
- Mean Absolute Error (MAE)
- R² Score

Training and Validation Loss curves were also analyzed to monitor model convergence and detect overfitting.

---

# 📊 Key Business Insights

Some important insights discovered during analysis include:

- Customer response time significantly impacts satisfaction.
- Certain product categories consistently receive lower CSAT scores.
- Experienced support agents generally achieve higher customer satisfaction.
- Longer handling times are associated with reduced customer satisfaction.
- Agent shift patterns influence customer experience.
- Customer support category and sub-category strongly affect overall CSAT.

These insights can help businesses optimize customer service operations and improve customer retention.

---

# 🌐 Flask Deployment

The trained ANN model was deployed using Flask.

Deployment workflow:

```
User Input

↓

Data Preprocessing

↓

Feature Scaling

↓

ANN Model Prediction

↓

Predicted CSAT Score
```

The Flask application provides real-time customer satisfaction predictions through a simple web interface.

---

# 📂 Project Structure

```
DeepCSAT/
│
├── Dataset/
│      eCommerce_Customer_support_data.csv
│
├── Notebook/
│      DeepCSAT.ipynb
│
├── Flask/
│      app.py
│      templates/
│      static/
│
├── Model/
│      csat_model.h5
│
├── README.md
│
└── requirements.txt
```

---

# 🚀 How to Run

Clone the repository

```bash
git clone https://github.com/yourusername/DeepCSAT.git
```

Install dependencies

```bash
pip install -r requirements.txt
```

Run Flask

```bash
python app.py
```

Open

```
http://127.0.0.1:5000
```

---

# 📌 Future Improvements

- Deploy using Docker
- Deploy on AWS / Azure
- Improve feature engineering
- Integrate NLP sentiment analysis on customer remarks
- Experiment with XGBoost and LightGBM
- Build a Streamlit Dashboard
- Explain predictions using SHAP
- Implement CI/CD pipeline
---

# 📚 Learning Outcomes

Through this project, I gained practical experience in

- Deep Learning
- Artificial Neural Networks
- Feature Engineering
- Model Evaluation
- Hyperparameter Tuning
- Data Visualization
- Business Analytics
- Flask Deployment
- End-to-End Machine Learning Pipeline

---

# 👨‍💻 Author

**SARATHRAJ R**
Data Scientist | Data Analyst | Machine Learning Enthusiast

LinkedIn: https://www.linkedin.com/in/sarathraj-r-ds/

---

# ⭐ If you found this project useful

Please consider giving this repository a ⭐ on GitHub.

It motivates me to build and share more real-world Machine Learning and Data Science projects.
