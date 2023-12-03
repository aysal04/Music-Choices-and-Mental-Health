# SASYA - Mental Health Analysis based on Music Preferences

## CS550 - Machine Learning - Major Project REPORT

**Authors:**
- Kata Lakshmi Lasya, 12140880 (BTech, CSE, Third year)
- M. V. Kiran Sooraj, 12141000 (BTech, CSE, Third year)
- Pingili Sameeksha Reddy, 12141240 (BTech, EE, Honours in CSE, Third year)

**Keywords:**
- Convolution Neural Networks
- Decision Trees
- GaussianNB
- K-Nearest Neighbours
- Neural Networks
- Support Vector Machine
- Linear Discriminant Analysis

## Abstract

This project explores the potential of personal musical preferences as a non-invasive criterion for assessing an individual's mental and emotional well-being. Leveraging machine learning techniques, we aim to develop a practical tool for mental health assessment based on musical preferences, providing an accessible means for individuals to self-assess their mental health. The project combines two models: one for predicting music genre preferences and another for assessing mental health indicators. The dataset includes the GTZAN Audio Dataset for music genre prediction and the "mxmh survey results" dataset for mental health analysis.

## 1. Introduction and Problem Motivation

Personal preferences, such as those related to daily aspects like food, art, and music, can reflect an individual's mental and emotional state. This project focuses on analyzing musical preferences as a unique and accessible criterion for understanding psychological well-being. The project recognizes the potential of everyday choices, such as music preferences, to motivate individuals to seek professional help without undergoing lengthy and complex tests.

## 2. Datasets

### 2.1 GTZAN Audio Dataset

For music genre prediction, the renowned GTZAN audio dataset is employed. This dataset consists of ten distinct music genres, each composed of precisely one hundred audio tracks. The genres include blues, classical, country, disco, hiphop, jazz, metal, pop, reggae, and rock.

### 2.2 MXMH Survey Results Dataset

For mental health analysis, the dataset is sourced from Kaggle, specifically the "mxmh survey results" dataset. This comprehensive dataset captures diverse factors influencing an individual's mental health, including age, hours dedicated to music consumption, frequency of exposure to different music genres, and preferred music genre.

## 3. Solution Approach

### 3.1 Input from User

A form asks basic questions about the user's lifestyle, including age, hours per day listening to music, instrumentalist or composer status, favorite music genre, exploratory attitude towards music, knowledge of foreign languages, and beats per minute of the heart. Additionally, the user provides five audio clips of their current favorite music.

### 3.2 Music Genre Prediction Model

The initial usage of 30-second audio clips was disregarded in favor of 3-second audio clips, resulting in an improved CNN model with 91.08% accuracy. The music genre prediction model evaluates each audio clip, providing a probabilistic genre prediction spectrum.

### 3.3 Mental Health Prediction Model

The input for the mental health prediction model is based on the user's degree of liking towards a genre. The output of the music prediction model is mapped to different mental health conditions. Various models are used for different mental health indicators: KNN for depression, Decision Tree for anxiety and insomnia, and SVM for OCD.

## 4. Uniqueness

The project's uniqueness lies in its integration of music preferences and lifestyle choices to predict mental health outcomes. The solution improves accuracy by analyzing the user's current favorite songs in conjunction with self-awareness-based responses.

## 5. Results and Evaluation

### 5.1 Music Genre Prediction Model

- KNN: 64.50% accuracy
- SVM: 67% accuracy
- Ensemble of SVM: 64% accuracy
- CNN with 3 hidden layers: 91.08% accuracy

### 5.2 Mental Health Prediction Model

- Depression (KNN): 64.09% accuracy
- Anxiety (Decision tree): 57% accuracy
- Insomnia (Decision tree): 72.93% accuracy
- OCD (SVM): 84.53% accuracy

## 6. Scope of Improvement

The project can be improved by revisiting the mental health prediction model for better accuracy, exploring alternative model types, and collecting better datasets for mental health prediction.

## 7. References

1. [Stanford CS229 Project Report](https://cs229.stanford.edu/proj2018/report/21.pdf)
2. [Predicting Depression Based on Musical Taste](https://macuriels.com/project/predicting-depression-with-music/) by Miguel Curiel

**Note:** The output of the model should be considered as a prediction only, and users are encouraged to consult with trained professionals for mental health validation.

---
**Project Overview**

This project overview summarizes the current progress, challenges, and future tasks. The authors plan to revisit the mental health prediction model for improved accuracy, streamline individual models for a unified system, and develop a basic web interface for user-friendly predictions. The ultimate goal is to deliver a web application that predicts mental health based on lifestyle and music choices with enhanced accuracy.

*Phase 2 Implemented as of 2023-12-04*

