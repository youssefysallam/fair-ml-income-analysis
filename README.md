# Fair ML Income Analysis

This repository contains a machine learning and fairness analysis project focused on the **UCI Adult Income dataset**. The project studies how standard machine learning models perform on income prediction tasks and evaluates whether these models exhibit **systematic bias across demographic groups**, with a particular focus on gender and race.

Using the Adult dataset, which contains census-based attributes and a binary income label (≤50K or >50K), the project trains baseline models and evaluates both **predictive performance** and **fairness metrics**. The goal is to highlight how high accuracy does not necessarily imply fair outcomes and to explore mitigation strategies that attempt to reduce observed disparities.

The repository includes data preprocessing, modeling code, fairness evaluation, visualizations, and a final research report written in LaTeX.

---------------------------------------------------------------------------------------------------------------------------------------------------------

## 📁 Repository Structure
```text
fair-ml-income-analysis/
|   README.md (this file 😊)
|   requirements.txt
|
+---data
|       adult.csv
|       baseline_results.csv
|       metrics_comparison.csv
|       mitigation_results.csv
|
+---notebooks
|   |   01_data_exploration.ipynb
|   |
|   \---.ipynb_checkpoints
|           01_data_exploration-checkpoint.ipynb
|
\---reports
    |   .gitignore
    |
    +---latex
    |   |   main.tex
    |   |   references.bib
    |   |
    |   \---figures
    |           accuracy_comparison.png
    |           dp_gap_comparison.png
    |           eo_gap_comparison.png
    |           gender_distribution.png
    |           income_by_gender_raw.png
    |           income_distribution.png
    |
    \---results
            Fair_ML_Income_Analysis_Final_Report.pdf

---------------------------------------------------------------------------------------------------------------------------------------------------------

## 📌 Folder Overview

### **data/**
Contains all dataset files used for training and evaluation, as well as CSV outputs generated during analysis.

- `adult.csv`: raw UCI Adult Income dataset used for model training  
- `baseline_results.csv`: evaluation metrics for the baseline model  
- `metrics_comparison.csv`: comparison of performance and fairness metrics across models  
- `mitigation_results.csv`: results after applying bias mitigation strategies  


### **notebooks/**
Jupyter notebooks documenting the workflow, including:
- data exploration and preprocessing  
- model training  
- fairness metric computation and analysis  

These notebooks provide transparency into the modeling and evaluation process and allow results to be reproduced.


### **reports/**
Materials related to analysis outputs and reporting.

- `reports/results/`: finalized research artifacts  
  - `Fair_ML_Income_Analysis_Final_Report.pdf`: compiled final research paper  


#### **reports/latex/**
This directory contains the **LaTeX source** used to generate the final research paper.

- `main.tex`: main LaTeX document  
- `references.bib`: bibliography file  
- `figures/`: all figures referenced by LaTeX (stored locally to avoid path issues during compilation)  


### **requirements.txt**
Python dependencies required to run the notebooks and reproduce all experiments and figures.


### **README.md**
Project overview, setup instructions, and repository documentation.

---------------------------------------------------------------------------------------------------------------------------------------------------------

## 🧠 Project Summary

Machine learning systems are increasingly deployed in high-stakes decision-making contexts such as hiring, lending, and criminal justice. This project evaluates whether income prediction models trained on real-world census data produce **unequal outcomes across demographic groups**.

The analysis:
- trains baseline classification models on the Adult dataset
- evaluates accuracy and standard performance metrics
- computes fairness metrics such as demographic parity and equal opportunity
- examines trade-offs between predictive performance and fairness

The final report summarizes findings and discusses the limitations of simple mitigation strategies.

---------------------------------------------------------------------------------------------------------------------------------------------------------

## 📦 Requirements

All required Python dependencies are listed in `requirements.txt`.

Install them using:

```bash
pip install -r requirements.txt
