# Mental Choices and Mental Health

## Project Overview

This project aims to explore the correlation between an individual's mental health and their music preferences. Leveraging the power of machine learning, we delve into two primary aspects: predicting an individual's favorite music genre and assessing their mental health based on lifestyle choices and music taste.

## 1. Data Pre-processing

### Model 1: Music Genre Prediction

**Data:** GTZAN Audio Dataset - 10 genres, 100 audio files each (30 seconds duration)

**Pre-processing:**
- Genre vs Duration and Genre vs No. of Tracks plots
- Sampled signal plot for one audio track
- Generating spectrogram using the 'inferno' color map
- Extracting audio features: mean, variance, standardizing with StandardScaler

### Model 2: Mental Health Prediction

**Data:** MXMH Survey Results Dataset

**Pre-processing:**
- Replacing null values with mode
- Distribution analysis of primary streaming services, age, hours per day, BPM
- Removing outliers in age, hours per day, BPM
- Heat map analysis

## 2. Training and Validation

### Model 1: Music Genre Prediction

**Models Trained:**
- KNN (64.50% accuracy)
- SVM (67% accuracy)
- Ensemble of SVM (64% accuracy)
- CNN (2 hidden layers, 74% accuracy)
- CNN (3 hidden layers, 61% accuracy)
- CNN (5 hidden layers, 69.5% accuracy)

**Best Model:**
- CNN with 3 hidden layers (91.08% accuracy) on 3-second audio samples

### Model 2: Mental Health Prediction

- SVM, KNN, Linear Regression, Random Forests used
- Model performance disappointing, negative R2 error for depression prediction
- Revisiting data processing and exploring other model types

## 3. Tasks for Final Submission

1. Revisit Mental Health Prediction model for improved accuracy.
2. Streamline individual models to create a unified system.
3. Develop a basic web interface for user-friendly predictions.

## 4. Challenges and Action Plan

- **Challenge:** Disappointing performance in Mental Health Prediction model.
- **Action:** Revisit data processing, one-hot encoding, and explore alternative model types.

## 5. Final Deliverables

-A web application predicting mental health based on lifestyle and music choices with improved accuracy.

**Project Authors:**
-
- Kata Lakshmi Lasya, 12140880
- M. V. Kiran Sooraj, 12141000
- Pingili Sameeksha Reddy, 12141240

---

*Phase 1 Implemented as of 2023-11-09*
