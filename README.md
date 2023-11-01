
# AI_PHASE_5

# AI-Driven Exploration and Prediction of Company Registration Trends with RoC

## Table of Contents

- [Overview](#overview)
- [Dependencies](#dependencies)
- [Installation](#installation)
- [Usage](#usage)
- [Data Preparation](#data-preparation)
- [Training the Model](#training-the-model)
- [Making Predictions](#making-predictions)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Overview

This repository contains code for an AI-driven exploration and prediction system to analyze Company Registration Trends using data from the Registrar of Companies (RoC). It includes data preparation, model training, and prediction components, all designed to help you gain insights and forecast trends in company registrations.

## Dependencies

Before you begin, make sure you have the following dependencies installed:

- Python 3.x
- Jupyter Notebook (for running the notebooks)
- Required Python libraries (install them via `pip`):
  - pandas
  - numpy
  - scikit-learn
  - matplotlib
  - seaborn
  - ...

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

## Usage

To use this code, follow these steps:

### Data Preparation

1. Obtain the RoC dataset: [https://tn.data.gov.in/resource/company-master-data-tamil-nadu-upto-28th-february-2019].

2. Preprocess the dataset as needed using the provided scripts or customize them for your data format.

### Model

The Random forest Classifier model is used.

### Dataset splitting
 The cleaned data set is splitted into two parts, one for training and other for evaluating the model
 the x and y columns are,

 ```
X = df_encoded.drop(['COMPANY_CLASS'], axis=1)
y = df_encoded['COMPANY_CLASS']
```

 Dataset is splitted by,

 ```
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)

```

### Model Training

The model is trained using one set of splittrd data

```
rf_classifier.fit(X_train, y_train)

```
### model Prediction
To make predictions on the test data
```
y_pred = rf_classifier.predict(X_test)
```
## model evaluation
the model
```
accuracy = accuracy_score(y_test, y_pred)
conf_matrix = confusion_matrix(y_test, y_pred)
class_report = classification_report(y_test, y_pred)
```

## Results

```
accuracy_percentage = accuracy * 100
print(f'Accuracy: {accuracy_percentage:.2f}%')
```

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

## License

[Specify the license under which your code is released. Common options include MIT, Apache 2.0, or GPLv3.]

---

Feel free to customize this README according to your project's specific needs and provide additional information or resources as necessary. A well-structured README will help users understand how to run your code and make the most of your AI-driven exploration and prediction system for Company Registration Trends with RoC.
