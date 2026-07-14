# EMG Hand Gesture Classification using Classical Machine Learning

A beginner-friendly end-to-end machine learning pipeline for **surface
Electromyography (sEMG) hand gesture classification** using data
collected from the **Myo Thalmic armband**.

This project demonstrates the complete workflow of an EMG classification
system, beginning with exploratory data analysis and signal
interpretation, followed by feature extraction, dimensionality
reduction, and machine learning classification. Rather than focusing
solely on model performance, the project emphasizes understanding the
reasoning behind each processing step and the role of EMG signal
processing in gesture recognition.

## Project Overview

The dataset consists of raw EMG recordings collected from **36
subjects** wearing an **8-channel Myo Thalmic armband** while performing
seven static hand gestures. Since raw EMG signals are continuous
time-series data, they cannot be directly used by traditional machine
learning algorithms. Instead, the signals are segmented into
fixed-length windows, transformed into descriptive statistical features,
and used to train gesture classification models.

The notebook follows a complete EMG processing pipeline while explaining
the purpose of each stage, making it suitable for students and engineers
beginning work in biomedical signal processing.

## Pipeline

-   Dataset exploration and quality assessment
-   Class and subject distribution analysis
-   Raw EMG signal visualization
-   Channel activation comparisons across subjects and gestures
-   Correlation analysis between EMG channels
-   Power Spectral Density (PSD) analysis using Welch's method
-   Frequency-domain interpretation and preprocessing discussion
-   Feature extraction using sliding windows
    -   Mean Absolute Value (MAV)
    -   Root Mean Square (RMS)
    -   Variance (VAR)
-   Feature standardization
-   Principal Component Analysis (PCA)
-   Subject-wise train/test split
-   Classification using:
    -   Random Forest
    -   Logistic Regression
-   Model evaluation using:
    -   Accuracy
    -   Precision
    -   Recall
    -   F1-score
    -   Confusion Matrix

## Dataset

-   **Subjects:** 36
-   **EMG Channels:** 8
-   **Sampling Rate:** 200 Hz
-   **Gestures:**
    -   Rest
    -   Fist
    -   Wrist Flexion
    -   Wrist Extension
    -   Radial Deviation
    -   Ulnar Deviation
    -   Extended Palm

## Key Learning Outcomes

This project explores several fundamental concepts in EMG signal
processing and classical machine learning, including:

-   Time-series preprocessing
-   Sliding window segmentation
-   Feature engineering for biosignals
-   Signal visualization in both time and frequency domains
-   Channel correlation analysis
-   Subject-independent model evaluation
-   Feature scaling and dimensionality reduction
-   Comparison of classical machine learning models

## Technologies Used

-   Python
-   NumPy
-   Pandas
-   Matplotlib
-   Seaborn
-   SciPy
-   scikit-learn
-   Jupyter Notebook

## Future Improvements

-   Butterworth band-pass filtering
-   Additional EMG features (Waveform Length, Zero Crossings, Slope Sign
    Changes, Integrated EMG)
-   Feature selection techniques
-   Hyperparameter optimization
-   Deep learning approaches (CNN/LSTM)
-   Real-time EMG gesture recognition
-   Assistive rehabilitation applications for lower-limb movement
    intention detection

## Motivation

This project was developed as a self-directed learning exercise to gain
practical experience in biomedical signal processing and classical
machine learning. The long-term goal is to build toward more advanced
research in EMG-based assistive technologies, rehabilitation robotics,
and human-machine interaction.
