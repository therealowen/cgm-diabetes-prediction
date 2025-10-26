# Continuous Glucose Monitoring Data Analysis

This repository contains the analysis of continuous glucose monitoring (CGM) data for predicting type 2 diabetes mellitus in patients at risk.

## Description

This project implements Detrended Fluctuation Analysis (DFA) and other machine learning techniques to predict type 2 diabetes mellitus. The analysis uses continuous glucose monitoring data from patients at risk, with clinical metadata including gender, age, BMI, basal glycemia, HbA1c, and follow-up information.

## Dataset

- **S1/**: Contains 208 individual patient CGM data files (case 1.csv to case 208.csv)
- **clinical_data.txt**: Clinical metadata for all patients including:
  - Gender (0 = male, 1 = female)
  - Age (years)
  - Body mass index (Kg/m²)
  - Basal glycemia (mg/dL)
  - HbA1c (%)
  - Follow-up (days)
  - Final diagnosis of type 2 diabetes mellitus

## Analysis

The main analysis is performed in `S1-Phase1.ipynb`, which includes:

1. Data loading and preprocessing
2. Descriptive statistics for clinical and glucose data
3. Feature extraction from CGM time series
4. Model development and optimization
5. Comparison with other prediction metrics

## Reference

This work is based on the research paper:
> Detrended Fluctuation Analysis in the prediction of type 2 diabetes mellitus in patients at risk: Model optimization and comparison with other metrics
> 
> [PLOS ONE Publication](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0225817)

## Installation

1. Clone this repository:
```bash
git clone https://github.com/therealowen/cgm-diabetes-prediction.git
cd cgm-diabetes-prediction
```

2. Create a virtual environment:
```bash
python3 -m venv cgm-env
```

3. Activate the virtual environment:
```bash
source cgm-env/bin/activate  # On macOS/Linux
```

4. Install required packages:
```bash
pip install -r requirements.txt
```

## Usage

1. Activate the virtual environment (if not already activated):
```bash
source cgm-env/bin/activate
```

2. Open `S1-Phase1.ipynb` in Jupyter Notebook to run the analysis:
```bash
jupyter notebook
```