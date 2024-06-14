
# TURKFACT

TURKFACT is a multi-class machine learning model designed to fact-check Turkish text content. Developed to address the challenges posed by the rapid dissemination of misinformation and disinformation in the digital age, TURKFACT utilizes advanced natural language processing (NLP) and machine learning (ML) techniques to classify Turkish text into five categories: literary text, weather forecast, parody content, real content, and fake news.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Dataset](#dataset)
- [Model Training](#model-training)
- [Performance](#performance)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Introduction

In an era dominated by information overflow, discerning the authenticity of news and claims has become increasingly challenging. TURKFACT aims to provide a robust solution to this problem by leveraging machine learning models to detect complex linguistic patterns associated with misleading and divisive content in Turkish texts.

The project was developed by Fatih Sinan Esen and Sahin Emrah Amrahov from the Department of Computer Engineering at Ankara University, Türkiye.

## Features

- **Multi-class classification**: Classifies Turkish text into five distinct categories.
- **Advanced NLP techniques**: Utilizes Bag-of-Words (BoW) and Term Frequency-Inverse Document Frequency (TF-IDF) for text representation.
- **Comprehensive dataset**: Includes a rich corpus of 9,792 labeled texts.
- **Hyperparameter optimization**: Employs RandomizedSearchCV, GASearchCV, and GridSearchCV for optimal model performance.
- **High performance**: Achieves superior accuracy and reliability in identifying fake news and other categories.

## Installation

To use TURKFACT, you need to have Python installed on your system. You can install the necessary dependencies using the following commands:

```bash
git clone https://github.com/fatihsinanesen/TURKFACT.git
cd TURKFACT
pip install -r requirements.txt
```

## Usage

The project includes a Jupyter notebook (`main.ipynb`) that demonstrates how to use the TURKFACT model. To run the notebook:

```bash
jupyter notebook main.ipynb
```

The notebook guides you through the steps of loading the dataset, preprocessing the data, training the model, and evaluating its performance.

## Dataset

The dataset used in this project consists of 9,792 labeled Turkish texts categorized into five classes:

- **Literary Text**: 1,194 samples
- **Weather Forecast**: 777 samples
- **Parody Content**: 3,469 samples
- **Real Content**: 3,630 samples
- **Fake Content**: 722 samples

The data was collected from various online sources, including social media and fact-checking websites such as Teyit.org.

## Model Training

TURKFACT employs several classifiers for model training, including:

- Naive Bayes (Multinomial, Gaussian, Bernoulli)
- K-Nearest Neighbors (KNN)
- Logistic Regression
- Decision Tree
- Random Forest
- Support Vector Machine (SVM)
- eXtreme Gradient Boosting (XGBoost)

The model training process involves:

1. **Preprocessing**: Cleaning and transforming the text data.
2. **Feature Extraction**: Using BoW and TF-IDF techniques.
3. **Training**: Applying different classifiers to the processed data.
4. **Hyperparameter Optimization**: Fine-tuning the model parameters for optimal performance.

## Performance

The TURKFACT model achieves high accuracy and reliability across various metrics. The XGBoost classifier emerged as the best performing model with the following metrics:

- **Test Accuracy**: 0.93
- **Precision**: 0.93
- **Recall**: 0.93
- **F1 Score**: 0.93
- **AUC**: 0.99

These results highlight TURKFACT's effectiveness in accurately classifying Turkish text content.

## Contributing

Contributions to TURKFACT are welcome. If you have any suggestions, bug reports, or feature requests, please open an issue or submit a pull request.

## License

This project is licensed under the MIT License.

## Acknowledgments

We would like to thank the Department of Computer Engineering at Ankara University for their support. Special thanks to all contributors and researchers who have provided valuable insights and data for this project.
