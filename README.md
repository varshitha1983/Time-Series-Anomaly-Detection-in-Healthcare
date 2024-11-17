# **Anomaly Detection in Healthcare Time-Series Data**

---

## **Project Overview**
This project aims to address the critical challenge of anomaly detection in healthcare time-series data, focusing on the detection of irregularities in ECG signals. Anomalies in such data often indicate potential health issues, such as arrhythmias, which require timely identification. The study leverages the **ECG5000 dataset** and evaluates the performance of three deep learning models:

1. **LSTM Autoencoders**: Specialized for capturing sequential dependencies in time-series data.
2. **Standard Autoencoders**: Simple yet effective for static anomalies.
3. **Variational Autoencoders (VAEs)**: Employ probabilistic modeling for uncertainty estimation.

The results are benchmarked against other healthcare datasets to assess the models’ generalizability and effectiveness in real-world applications.

---

## **Key Features**
- Comparative analysis of **LSTM Autoencoders**, **Standard Autoencoders**, and **VAEs** for anomaly detection.
- Implementation of threshold-based anomaly classification using reconstruction errors.
- Evaluation on **multiple datasets** (ECG5000, MIT-BIH Arrhythmia, PhysioNet Challenge, Yahoo Anomaly Detection).
- Generation of key performance metrics, including **Accuracy**, **Precision**, **Recall**, **F1 Score**, and **ROC-AUC**.
- Real-time anomaly detection suitability assessment for healthcare applications.

---

# Training Results

This section presents the results and analyses from the training of the LSTM Autoencoders and Standard Autoencoders on the ECG5000 dataset.

---

## **Training Loss Curves**

### LSTM Autoencoders:
<img src="images/trainloss-lstm.png" alt="Training Loss Curve for LSTM Autoencoders" width="500">

### Standard Autoencoders:
<img src="images/loss-ae.png" alt="Training Loss Curve for Standard Autoencoders" width="500">

---

## **Loss Value Distributions**

### LSTM Autoencoders (10 Epochs):
- **Normal Data:**
  <img src="images/normalloss-lstm.png" alt="Loss Distribution for Normal Data - LSTM" width="400">

- **Anomalous Data:**
  <img src="images/anomalyloss-ae.png" alt="Loss Distribution for Anomalous Data - LSTM" width="400">

### Standard Autoencoders (28 Epochs):
- **Normal Data:**
  <img src="images/normalloss-lstm.png" alt="Loss Distribution for Normal Data - AE" width="400">

- **Anomalous Data:**
  <img src="images/anomalyloss-ae.png" alt="Loss Distribution for Anomalous Data - AE" width="400">

---

## **Reconstruction Errors**

Reconstruction errors for Standard Autoencoders are shown below:

- **Normal Data Reconstruction Errors:**
  <img src="images/normalre-ae.png" alt="Reconstruction Errors for Normal Data - AE" width="400">

- **Anomalous Data Reconstruction Errors:**
  <img src="images/anomalyre-ae.png" alt="Reconstruction Errors for Anomalous Data - AE" width="400">

---

## **Result Comparison**

Results obtained from three different models are summarized below:
<img src="images/results-compare.png" alt="Result Comparison Across Models" width="500">

---

### Notes
- All loss value distributions and reconstruction errors are based on the dataset splits for normal and anomalous data.
- The result comparison provides a quantitative evaluation of the three models, highlighting the LSTM Autoencoder's superiority in accuracy and other metrics.


