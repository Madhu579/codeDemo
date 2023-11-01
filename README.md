
# Artificial Intelligence 

# AI-Driven Exploration and Prediction of Company Registration Trends with RoC

## Table of Contents

- [Overview](#overview)
- [Dependencies](#dependencies)
- [Installation](#installation)
- [Usage](#usage)


## Overview

This repository contains code for an AI-driven exploration and prediction system to analyze Company Registration Trends using data from the Registrar of Companies (RoC). It includes data preparation, model training, and prediction components, all designed to help you gain insights and forecast trends in company registrations.

## Dependencies

Before you begin, make sure you have the following dependencies installed:

- Python installed
- Jupyter Notebook (for running the notebooks)
- Required Python libraries (install them via `pip`):
  - pandas
  - numpy
  - scikit-learn
  - matplotlib
  - seaborn
- dataset: [https://tn.data.gov.in/resource/company-master-data-tamil-nadu-upto-28th-february-2019].

## Installation

1. Clone the repository to your local machine:

   ```bash
   git clone https://github.com/MadhuMalathiBN/NaanMudhalvan.git
   cd NaanMudhalvan
   ```

2. Install the required Python packages:

   ```bash
   pip install -r requirements.txt
   ```

## Data set Source

 RoC dataset: [https://tn.data.gov.in/resource/company-master-data-tamil-nadu-upto-28th-february-2019].
 
## Usage

To use this code, follow these steps:

This project involves analyzing and visualizing data related to companies in Tamil Nadu, India. 
It uses Python libraries like Pandas, NumPy, Matplotlib, Seaborn, and scikit-learn to perform data processing, exploration, and machine learning.

## Usage

The code provided in this repository can be used to:

1. Load the dataset from a CSV file (Data_Gov_Tamil_Nadu.csv).
2. Data preprocessing:
   - Remove duplicate records.
   - Remove rows with missing values.
   - Data standardisation
   - Data type conversion
3. Save the cleaned dataset to a new CSV file (CleanesDataFile.csv).
4. Perform data analysis and visualization, including:
   - Descriptive statistics using Pandas.
   - Count the values of the "PAIDUP_CAPITAL" and "INDUSTRIAL_CLASS" columns.
   - Create various plots and visualizations using Matplotlib and Seaborn.
5. Train a Random Forest Classifier to predict the "COMPANY_CLASS" based on the dataset.
6. Evaluate the model's performance by calculating accuracy, generating a confusion matrix, and creating a classification report.

## Prerequisites

Before running the code, you need to have Python installed, and you should install the following Python packages using pip:

`bash
pip install pandas numpy scikit-learn matplotlib seaborn


## Contributing

If you'd like to contribute to this project, please follow these steps:

1. Fork the repository on GitHub.

2. Clone your fork locally and create a new branch for your work:

   ```bash
   git checkout -b feature/your-feature-name
   ```

3. Make your changes, commit them, and push to your fork:

   ```bash
   git commit -m "Your commit message"
   git push origin feature/your-feature-name
   ```

4. Create a pull request from your fork to the main repository.


