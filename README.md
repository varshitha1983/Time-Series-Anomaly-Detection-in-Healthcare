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

## **Training Results**
The training loss curve is shown below:
<img src="images/train-lstm.png" alt="Training Loss Curve for LSTM Autoencoders" width="500">
<img src="images/loss-ae.png" alt="Training Loss Curve for Standard Autoencoders" width="500">
Below are the Distribution of Loss values using LSTM Autoencoders for 10 epochs:
<img src="images/normalloss-lstm.png" alt="Training Loss Curve for LSTM Autoencoders" width="500">
<img src="images/anomalyloss-ae.png" alt="Training Loss Curve for LSTM Autoencoders" width="500">
Below are the Distribution of Loss values using Standard Autoencoders for 28 epochs:
<img src="images/normalloss-lstm.png" alt="Training Loss Curve for LSTM Autoencoders" width="500">
<img src="images/anomalyloss-ae.png" alt="Training Loss Curve for LSTM Autoencoders" width="500">

---

## **Reeconstruction Errors**
Below figures shows the reconstruction errors for Standard Autoencoders:
<img src="images/normalre-ae.png" alt="Training Loss Curve for LSTM Autoencoders" width="500">
<img src="images/aomalyre-ae.png" alt="Training Loss Curve for LSTM Autoencoders" width="500">

---

## **Result Comparison**
Results obtained fro three different models are illustrated below:
<img src="images/results-compare.png" alt="Training Loss Curve for LSTM Autoencoders" width="500">
