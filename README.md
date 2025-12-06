# cyber-attack-detection-MLP-GRU
🚨 Cyber Attack Detection using MLP + GRU

A deep learning project built to classify network traffic into four cybersecurity categories using a hybrid MLP + GRU neural network.

📌 Overview

This project focuses on detecting different cyber activities using machine learning.
The model predicts 4 classes:

normal – safe network activity

nss – possible Network Security Scan

qc – quarantined/suspicious connection

zt – zero-trust flagged traffic

The project includes:

Data cleaning

Exploratory data analysis (EDA)

Feature preprocessing

Deep learning model (MLP + GRU)

Training, evaluation, and visualization

Saved model in .joblib format

Notebook (.ipynb) and HTML version

🧠 Technologies Used

Python

TensorFlow / Keras

Pandas & NumPy

Scikit-learn

Matplotlib & Seaborn

Joblib

Jupyter Notebook

🗂️ Project Structure
cyber-attack-detection-MLP-GRU/
│── MLP-GRU.ipynb            # Jupyter Notebook
│── MLP-GRU.html             # HTML exported version
│── models/
│     └── model.joblib       # Saved trained model
│── requirements.txt         # Dependencies
│── README.md                # Project documentation
│── .gitignore

🔍 Dataset Description

The dataset contains network traffic logs with features like:

duration

orig_bytes

resp_bytes

orig_packets

resp_packets

class (target variable)

⚠️ Full dataset not included here due to size.
A small sample or dataset link can be added if needed.

🧹 Preprocessing Steps

Handled null values

Removed outliers

Applied feature scaling

Encoded categorical labels

Split dataset (train/test)

Reshaped input for GRU layer

🧱 Model Architecture (MLP + GRU)

The model combines:

MLP layers → for feature extraction

GRU layer → to learn sequential patterns

Dense softmax → for 4-class classification

Advantages:

Learns both numerical and temporal characteristics

Good for cyber-traffic patterns

🚀 How to Run This Project
1. Clone the repository
git clone https://github.com/<your-username>/<repo-name>.git

2. Install dependencies
pip install -r requirements.txt

3. Open the notebook
jupyter notebook MLP-GRU.ipynb

📦 Load the Saved Model (.joblib)

To load and use the saved trained model:

import joblib

model = joblib.load("models/model.joblib")

# Example: prediction
y_pred = model.predict(X_test)
print(y_pred)

📊 Results

(Add these after you upload your images/metrics)

Training accuracy: XX%

Validation accuracy: XX%

Confusion matrix

Loss & accuracy graphs

Class-wise performance

You can upload plots as PNG images into GitHub and insert them here.

🔮 Future Improvements

Add LSTM or Bidirectional GRU variant

Deploy model using Flask/FastAPI

Real-time intrusion detection demo

Convert model to ONNX

Integrate federated learning version

🏁 Conclusion

This project demonstrates:

✔ Data cleaning & preprocessing
✔ Deep learning (MLP + GRU)
✔ Cybersecurity domain understanding
✔ Model evaluation
✔ Real-world ML pipeline

A perfect project for ML Engineer, Cybersecurity Analyst, and AI Engineer portfolios.
