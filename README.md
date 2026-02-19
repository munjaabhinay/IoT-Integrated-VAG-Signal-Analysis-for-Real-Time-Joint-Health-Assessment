# IoT-Integrated VAG Signal Analysis for Real-Time Joint Health Assessment

**Overview**

This project presents an IoT-enabled joint health monitoring system using Vibroarthrography (VAG) signal analysis. The system captures vibration signals from the knee joint using wearable MEMS sensors and applies machine learning techniques to classify joint conditions in real time.

The solution provides a non-invasive, portable, and cost-effective approach for early detection of joint abnormalities, supporting remote healthcare and preventive diagnosis.

**Key Features**

    Real-time VAG signal acquisition using MEMS accelerometer (MPU6050 / ADXL345)
    
    Signal preprocessing (band-pass filtering, denoising, segmentation)
    
    Time-domain and frequency-domain feature extraction
    
    Machine learning-based joint classification (Healthy / Abnormal)
    
    IoT-based cloud transmission using ESP32 and MQTT/HTTP
    
    Web dashboard for visualization and monitoring

**Technologies Used**

  **Hardware**

    ESP32 (Wi-Fi enabled microcontroller)
    
    MEMS Accelerometer (MPU6050 / ADXL345)
    
    Li-ion battery / USB power supply
    
   **Software**
    
    Python
    
    NumPy, Pandas
    
    Scikit-learn
    
    TensorFlow/Keras (for CNN)
    
    Matplotlib
    
    Arduino IDE
    
    MQTT / Firebase / ThingSpeak

**Methodology**

  **Signal Acquisition**
      VAG signals are collected at 1 kHz sampling rate during knee movement.

  **Preprocessing**
  
    Band-pass filtering (50–250 Hz)
    
    Wavelet denoising
    
    Signal segmentation
    
    Normalization

  **Feature Extraction**

      RMS, Variance, Zero-crossing rate
      
      Spectral centroid, dominant frequency
      
      Wavelet-based features

  **Model Training**

      Support Vector Machine (SVM)
      
      Random Forest
      
      Convolutional Neural Network (CNN)
      
      Hybrid Model (SVC + KNN)

  **IoT Integration**

      Real-time data transmission via ESP32
      
      Cloud-based classification and storage
      
      Dashboard visualization

**Results**

    Hybrid SVC + KNN model achieved improved classification accuracy.
    
    System enables real-time detection of joint abnormalities.
    
    Provides low-latency (<2 seconds) feedback.
