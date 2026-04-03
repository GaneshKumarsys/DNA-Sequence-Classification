## Brief Introduction:

I am Ganeshkumar V, a Data Analyst with a B.Tech in Biotechnology.This project applies bioinformatics techniques and machine learning to classify human DNA sequences into gene families using k-mer feature extraction.

## Project Overview:

##### This repository contains the complete work for Human DNA Sequence Classification using the Human DNA dataset from Kaggle.

The project involves:

- Exploratory Data Analysis (EDA) on 3,629 human DNA sequences
- Nucleotide base frequency analysis (A, T, G, C) and GC content study
- K-mer feature extraction (k=4) — a real bioinformatics technique
- Building and comparing 5 machine learning classification models
- Identifying the best model for gene family prediction


## Objective:

#### To analyze human DNA sequences in order to:

>> Understand nucleotide base composition across 7 gene families
>> Validate Chargaff's rule through correlation analysis
>> Convert raw DNA strings into ML-ready features using k-mer counting
>> Classify sequences into gene families with maximum accuracy


## Dataset:

#### Dataset sourced from Kaggle:

 Kaggle: https://www.kaggle.com/datasets/nageshsingh/dna-sequence-dataset
 
 File used: human.txt (tab-separated)
 
 Records: 4,380 raw → 3,629 after duplicate removal
 
 Features: DNA sequence string + gene family class label (0–6)


## Gene Family Classes:
0 - G Protein Coupled Receptors  →  446 sequences

1 - Tyrosine Kinase               →  408 sequences

2 - Tyrosine Phosphatase          →  291 sequences

3 - Synthetase                    →  570 sequences

4 - Synthase                      →  590 sequences

5 - Ion Channel                   →  215 sequences

6 - Transcription Factor          → 1109 sequences

## Tools Used:

 Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn)

 Jupyter Notebook

 Git & GitHub

## Repository Structure:

Data/       → Raw human DNA dataset (human.txt)

Notebook/   → EDA, Feature Engineering & ML Notebook (.ipynb)

PNGs/  → EDA plots and model comparison screenshots

README.md   → Project Documentation

## Key Biological Findings:

* Chargaff's rule confirmed — A-T and G-C show strong negative correlation (-0.80 and -0.68 respectively) in the heatmap
* Mean GC content = 0.531 — Tyrosine Kinase has highest GC (0.559), Tyrosine Phosphatase has lowest (0.504)
* Transcription Factor is the most represented gene family (30.6%) Sequence lengths range from 5 to 18,921 bp — mean of 1,218 bp
* 751 duplicate sequences removed — data quality step confirmed


## ML Models & Results:
Model                   Accuracy

Random Forest           73.83%  ← Best Model

Gradient Boosting       69.28%

KNN                     68.46%

Logistic Regression     67.77%

Multinomial NB          37.05%

## Cross-Validation (Random Forest — 5 Fold):

> Fold Scores  : [50.41, 45.45, 50.55, 49.04, 45.52]
> Mean Accuracy: 48.19%
> Std Deviation: 2.27%

## Key Deliverables:

> Cleaned dataset with 751 duplicates removed

#### EDA visualizations:

- Gene family distribution (bar + pie chart)
- Sequence length distribution and boxplot by class
- Nucleotide base frequency histograms (A, T, G, C)
- GC content distribution and mean GC by gene family
- Correlation heatmap confirming Chargaff's rule
- Pairplot of nucleotide features by gene family


#### K-mer feature matrix:

-K = 4 (4-mers)
-256 unique features extracted
-Feature matrix shape: (3629, 256)


> Best model: Random Forest — 73.83% test accuracy

## Project Status:
-------- COMPLETED --------

## License

This project is licensed under the MIT License.
