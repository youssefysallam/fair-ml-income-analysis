# Fair ML Income Analysis

This repository contains a machine learning and fairness analysis project focused on the **UCI Adult Income dataset**. The project studies how standard machine learning models perform on income prediction tasks and evaluates whether these models exhibit **systematic bias across demographic groups**, with a particular focus on gender and race.

Using the Adult dataset, which contains census-based attributes and a binary income label (≤50K or >50K), the project trains baseline models and evaluates both **predictive performance** and **fairness metrics**. The goal is to highlight how high accuracy does not necessarily imply fair outcomes and to explore mitigation strategies that attempt to reduce observed disparities.

The repository includes data preprocessing, modeling code, fairness evaluation, visualizations, and a final research report written in LaTeX.

---------------------------------------------------------------------------------------------------------------------------------------------------------

## 📁 Repository Structure
fair-ml-income-analysis/
├── data/ # Dataset files used for training & CSV outputs used for tables and figures
│
├── notebooks/ # Jupyter notebooks for analysis and experiments
│ ├── data_cleaning.ipynb
│ ├── model_training.ipynb
│ └── fairness_evaluation.ipynb
│
├── reports/
│ ├── results/ # Research findings report
│ ├── Fair_ML_Income_Analysis_Final_Report.pdf
│ └── latex/ # LaTeX source code for the report
│ ├── main.tex
│ ├── references.bib
│ └── figures/ # Figures imported directly by LaTeX
│
│
├── requirements.txt # Python dependencies
└── README.md # Project overview (this file 😊)

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

Install dependencies with:

```bash
pip install -r requirements.txt
