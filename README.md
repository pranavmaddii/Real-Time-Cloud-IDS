# Real-Time Advanced Intrusion Detection in Cloud Networks

This project proposes a **hybrid Intrusion Detection System (IDS)** for cloud environments, combining 
Random Forest and Autoencoder models to detect both known and novel attacks in real time.  

- **Dataset:** NSL-KDD (5 selected features: duration, src_bytes, dst_bytes, count, serror_rate)  
- **Approach:** 
  - Random Forest for classifying known attack patterns  
  - Autoencoder for anomaly detection (novel threats)  
  - Hybrid weighted prediction to reduce false positives  
- **Deployment:** Streamlit-based web app with real-time monitoring and visualizations  

## 🚀 Features
- Real-time detection of intrusions with 99.3% accuracy  
- Dynamic thresholding to reduce false positives  
- Scalable cloud-ready deployment (tested on AWS EC2)  
- Lightweight feature selection for faster computation  
- User-friendly Streamlit dashboard with live predictions  

## 🛠 Tech Stack
- Python 3.8  
- TensorFlow / Keras (Autoencoder)  
- Scikit-learn (Random Forest)  
- Streamlit (Web App)  
- NSL-KDD Dataset  

## 📊 Results
- Accuracy: **99.3%**  
- Precision: **93%**  
- Recall: **91%**  
- SLA violations reduced to 3.9%  
- Latency: **0.5s per prediction**  

## 📂 Repository Structure
- `app.py` → Streamlit application  
- `utils.py` → Preprocessing & hybrid prediction logic  
- `random_forest.pkl` → Trained Random Forest model  
- `autoencoder.h5` → Trained Autoencoder model  
- `scaler.pkl` → Data normalization object  
- `autoencoder_threshold.pkl` → Dynamic anomaly detection threshold  

## 📌 Use Case
This system enhances **cloud network security** by providing proactive, real-time intrusion detection, 
making it suitable for applications like IoT sensor networks, e-commerce platforms, and enterprise cloud systems.
