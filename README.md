# 🔍 EDGAR Log Anomaly Detection using Spark & LSTM Autoencoder

This project implements a **Big Data Analytics pipeline** for detecting anomalies in EDGAR log files.  
It uses **Apache Spark** for distributed data processing and an **LSTM Autoencoder** (TensorFlow/Keras) to detect unusual access patterns.

---

## 📌 Project Overview

- 📂 **Input**: One month of EDGAR logs stored as multiple CSV files in Google Drive.
- ⚙️ **Processing**: PySpark handles ingestion, parsing, cleaning, and transformations.
- 🧠 **Modeling**: An LSTM Autoencoder learns normal log behavior.
- 🚩 **Output**: Flags anomalous log entries based on reconstruction error.

---

## ✅ Features

- **Full-month batch processing** of large CSV log files.
- Works with **Google Drive** as storage.
- Uses **PySpark DataFrame API** and **Spark SQL**.
- Trains a **Deep Learning Autoencoder** to detect anomalies.
- Supports saving intermediate results in **Parquet**.
- Visualizes anomaly scores with Matplotlib and Seaborn.

---

## ✅ Dependencies

# Install Java
apt-get install openjdk-11-jdk-headless -qq

# Download Spark 3.4.1
wget https://archive.apache.org/dist/spark/spark-3.4.1/spark-3.4.1-bin-hadoop3.tgz

# Extract Spark
tar -xzf spark-3.4.1-bin-hadoop3.tgz

# Install Python libraries
pip install findspark scikit-learn tensorflow pyarrow
