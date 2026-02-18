# Developing Test Bed for Screen Gleaning Attack on Smartphones for OTP Retrieval

Machine learning–based reconstruction of smartphone screen content from electromagnetic emissions using software-defined radio and signal processing techniques. This project demonstrates how side-channel leakage from display hardware can be modeled and decoded using supervised learning.

Developed as an M.Tech thesis at Indian Institute of Technology Kanpur in Association with **DRDO**(Defense Research and Development Organisation).

---

## Overview

This project builds an end-to-end pipeline to:

* Capture electromagnetic (EM) leakage from smartphone displays
* Process high-dimensional time-series signals
* Engineer frequency-domain features
* Train machine learning models to predict screen content
* Evaluate information leakage using statistical metrics

The system demonstrates the feasibility of recovering sensitive information such as OTP digits from EM emissions without direct device access.

---

## Problem Statement

Electronic devices unintentionally emit electromagnetic signals during operation. These signals may leak sensitive information. This project investigates:

* Whether screen content can be reconstructed from EM leakage
* How machine learning can decode signal patterns
* The security risks associated with side-channel leakage

---

## System Architecture

Pipeline:

1. **Signal Acquisition**

   * Capture EM emissions using Software Defined Radio (SDR)
   * Generate raw time-series signal data

2. **Signal Processing**

   * Fast Fourier Transform (FFT)
   * Noise filtering and normalization
   * Feature extraction

3. **Feature Engineering**

   * High-dimensional signal features (625K+)
   * Dimensionality reduction experiments
   * Statistical feature analysis

4. **Machine Learning Modeling**

   * Supervised classification models
   * Multi-class and binary prediction tasks

5. **Evaluation**

   * Classification accuracy
   * Signal-to-noise analysis
   * Leakage detection metrics

---

## Key Features

* End-to-end ML pipeline for EM signal classification
* High-dimensional time-series feature engineering
* Large-scale labeled dataset generation
* Multi-class screen content prediction
* Feature reduction experiments
* Statistical leakage analysis

---

## Machine Learning Models Used

* Support Vector Machine (SVM)
* Random Forest
* Decision Tree
* Binary and Multi-class classification approaches

Future work explores deep learning–based time-series models (RNNs).

---

## Dataset

The dataset consists of:

* Electromagnetic signal traces from smartphone displays
* Labeled screen content (digits, colors, patterns)
* Multiple experimental conditions and screen positions
* High-dimensional feature vectors extracted from FFT

Note: Due to research confidentiality, raw data and code are not publicly released. The thesis has been formally defended.

---

## Evaluation Metrics

* Classification Accuracy
* Signal-to-Noise Ratio (SNR)
* Normalized Inter-Class Variance (NICV)
* Test Vector Leakage Assessment (TVLA)

These metrics quantify signal separability and information leakage.

---

## Results

* Successful classification of screen content from EM signals
* Demonstrated feasibility of OTP digit prediction
* High separability of signal features across classes
* Improved computational efficiency through feature reduction

---

## Tech Stack

* Python
* NumPy
* SciPy
* scikit-learn
* Signal Processing (FFT)
* Software Defined Radio (SDR)
* Statistical Analysis

---

## Applications

* Side-channel security research
* Signal processing and time-series modeling
* Hardware security analysis
* Privacy risk assessment
* ML-based pattern recognition from physical signals

---

## Research Impact

This work demonstrates the potential of machine learning to extract sensitive information from unintended physical emissions and highlights the need for stronger countermeasures against electromagnetic leakage in modern devices.

---

## Author

Kakumanu Vamsee Krishna
M.Tech Research Project — Data Science, Machine Learning & Signal Processing

---
