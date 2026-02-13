# MiniProject – Network Intrusion Detection System (NIDS)

A Machine Learning–based Network Intrusion Detection System built using the CIC Intrusion Detection Dataset.
This project detects and classifies multiple types of cyber-attacks using supervised learning models.

## Project Overview

The objective of this project is to:

Detect malicious network traffic

Classify different attack types

Handle class imbalance

Compare multiple machine learning algorithms

Evaluate performance using classification metrics

## Dataset

The project uses the CIC Intrusion Detection Dataset, which contains labeled network traffic flows.

Attack Categories

BENIGN

Bot

DDoS

DoS GoldenEye

DoS Hulk

DoS Slowhttptest

DoS Slowloris

FTP-Patator

SSH-Patator

Heartbleed

Infiltration

PortScan

Web Attack – Brute Force

Web Attack – SQL Injection

Web Attack – XSS


## Data Preprocessing Pipeline

Load multiple CSV files from dataset directory

Merge datasets

Remove duplicate rows

Remove duplicate columns

Handle infinite values

Remove rows with missing values

Encode categorical features

Standardize numerical features

Apply oversampling to balance minority classes

Perform dimensionality reduction using PCA

After preprocessing:

Final dataset size after oversampling: 4,615,844 samples

Reduced to 10 principal components using PCA

Machine Learning Models Used

The following models were implemented and compared:

Decision Tree

Extra Trees Classifier

Random Forest

XGBoost

## Model Evaluation Metrics

Each model was evaluated using:

Accuracy

Precision

Recall

F1-Score

## Classification Report

Results Summary
**Decision Tree**

Accuracy: 99.81%

**Extra Trees Classifier**

Accuracy: 99.87%

**Random Forest**

Accuracy: 99.87%

**XGBoost**

Accuracy: 99.59%

Extra Trees and Random Forest performed best overall in terms of balanced precision and recall across attack categories.

## Key Techniques Used

Label Encoding

StandardScaler

RandomOverSampler (Imbalanced Learning)

Principal Component Analysis (PCA)

Ensemble Learning Methods

## Installation

Clone the repository:

git clone https://github.com/jibixn/MiniProject-NIDS.git
cd MiniProject-NIDS


Install dependencies:

pip install -r requirements.txt

## Technologies Used

Python

Pandas

NumPy

Scikit-learn

XGBoost

Imbalanced-learn

Matplotlib (optional for visualization)
