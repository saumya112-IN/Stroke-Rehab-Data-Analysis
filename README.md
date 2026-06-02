# AI-Driven Stroke Rehabilitation Analysis using Multimodal EEG

## Overview

Stroke is one of the leading causes of long-term disability worldwide, often affecting upper limb motor functions and reducing patients' quality of life. Effective rehabilitation requires continuous monitoring and assessment of motor recovery, which can be challenging using traditional clinical evaluations alone.

This project presents an AI-driven framework for analyzing electroencephalography (EEG) signals collected during upper limb rehabilitation exercises. Using a multi-paradigm EEG dataset, the system leverages deep learning techniques to identify motor-related neural patterns, classify rehabilitation tasks, and support the development of intelligent rehabilitation monitoring systems.

The project combines EEG signal processing, machine learning, and deep learning to create a scalable pipeline capable of handling large-scale rehabilitation datasets while providing insights into neural activity associated with motor recovery.

---

## Objectives

* Develop an end-to-end EEG analysis pipeline for stroke rehabilitation research.
* Process and analyze multi-paradigm EEG recordings collected during upper limb rehabilitation exercises.
* Build deep learning models capable of recognizing motor-related brain activity.
* Investigate temporal neural patterns associated with rehabilitation tasks.
* Create a foundation for future personalized rehabilitation recommendation systems.

---

## Dataset

**Dataset:** A Multi-Paradigm EEG Dataset for Studying Upper Limb Rehabilitation Exercises

The dataset contains EEG recordings collected during multiple rehabilitation paradigms, including motor imagery and motor execution tasks designed to study upper limb recovery and motor learning processes.

### Data Types

* Raw EEG Data (.set/.fdt format)
* Preprocessed EEG Data
* Event Annotations
* Multi-Session Recordings
* Multi-Subject Data

### Dataset Features

* Multi-paradigm rehabilitation exercises
* High-density EEG recordings
* Event-based annotations
* Suitable for BCI and neurorehabilitation research
* Publicly available for academic use

---

## Project Architecture

```text
Dataset Acquisition
        │
        ▼
Data Download & Extraction
        │
        ▼
EEGLAB Data Loading (.set/.fdt)
        │
        ▼
EEG Preprocessing
        │
        ▼
Event Extraction & Label Generation
        │
        ▼
Signal Segmentation
        │
        ▼
Feature Learning
        │
        ▼
CNN-LSTM Deep Learning Model
        │
        ▼
Classification & Evaluation
        │
        ▼
Model Interpretation & Visualization
```

---

## Methodology

### 1. Data Acquisition

* Automatic retrieval of dataset files from Figshare.
* Support for both raw and preprocessed EEG datasets.
* Automated extraction and organization of large archive files.

### 2. EEG Processing

* Loading EEGLAB (.set/.fdt) recordings using MNE.
* Extraction of event markers and annotations.
* Signal segmentation into fixed-length windows.
* Normalization and preparation for deep learning.

### 3. Deep Learning Model

A hybrid CNN-LSTM architecture is used to capture both spatial and temporal characteristics of EEG signals.

#### CNN Component

* Learns spatial EEG channel representations.
* Captures local neural activation patterns.
* Reduces noise and dimensionality.

#### LSTM Component

* Models temporal dependencies.
* Learns sequential brain activity patterns.
* Captures task-related neural dynamics.

---

## Technologies Used

### Programming

* Python

### Deep Learning

* PyTorch

### EEG Processing

* MNE-Python
* NumPy
* SciPy

### Machine Learning

* Scikit-Learn

### Data Handling

* Pandas
* Requests

### Visualization

* Matplotlib
* Seaborn

---

## Project Structure

```text
stroke-rehab-ai/
│
├── data/
│   ├── raw/
│   └── preprocessed/
│
├── notebooks/
│
├── src/
│   ├── data_loader.py
│   ├── preprocessing.py
│   ├── model.py
│   ├── train.py
│   └── evaluation.py
│
├── models/
│
├── results/
│
├── dashboard/
│
├── requirements.txt
│
└── README.md
```

---

## Model Training

### Input

* EEG Segments
* Event Labels

### Output

* Motor Task Classification
* Rehabilitation Exercise Recognition

### Training Configuration

* Framework: PyTorch
* Optimizer: Adam
* Loss Function: CrossEntropyLoss
* GPU Support: CUDA

---

## Future Enhancements

### Research Extensions

* EEG Transformer Models
* Attention-Based Architectures
* Self-Supervised Learning
* Contrastive Learning for EEG
* Multimodal Learning

### Clinical Applications

* Stroke Recovery Prediction
* Personalized Rehabilitation Planning
* Brain-Computer Interface Integration
* Clinical Decision Support Systems
* Real-Time Rehabilitation Monitoring

### Explainable AI

* SHAP-Based Interpretability
* EEG Channel Importance Analysis
* Feature Attribution Methods

---

## Potential Impact

This project demonstrates how artificial intelligence and neurotechnology can be combined to advance stroke rehabilitation research. By analyzing neural activity during rehabilitation exercises, the system aims to support clinicians and researchers in understanding motor recovery mechanisms and developing more personalized rehabilitation strategies.

---

## Skills Demonstrated

* Deep Learning
* EEG Signal Processing
* Biomedical Data Analysis
* Time-Series Modeling
* Neuroinformatics
* Healthcare AI
* Machine Learning
* PyTorch
* MNE-Python
* Research-Oriented Software Development

---

## Author

**Saumya Singh Jaiswal**

Master of Science in Computer Science
Artificial Intelligence • Healthcare AI • Biomedical Informatics • Computer Vision • Deep Learning

Passionate about leveraging AI and biomedical data to develop intelligent healthcare solutions that improve patient outcomes and advance precision medicine.
