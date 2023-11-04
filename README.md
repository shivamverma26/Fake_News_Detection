# Fake News Detection

Detecting Fake News with Natural Language Processing and Machine Learning in Python

## Overview

This project employs various natural language processing techniques and machine learning algorithms to classify fake news articles. Using scikit-learn libraries in Python, we aim to differentiate between legitimate and fabricated news.

## Getting Started

To set up and run this project on your local machine for development and testing, follow these steps:

### Prerequisites

Ensure you have the following:

1. **Python 3.6**: If not already installed, download Python from [python.org](https://www.python.org/downloads/) and set up PATH variables if necessary.
2. **Anaconda**: Alternatively, you can download Anaconda from [anaconda.com](https://www.anaconda.com/download/).
3. **Required Packages**: After installing Python or Anaconda, install the necessary packages by running the following commands:
   - If using Python 3.6:
     ```bash
     pip install -U scikit-learn
     pip install numpy
     pip install scipy
     ```
   - If using Anaconda, run these commands in Anaconda prompt:
     ```bash
     conda install -c scikit-learn
     conda install -c anaconda numpy
     conda install -c anaconda scipy
     ```

### Dataset

We use the LIAR dataset, originally designed for Fake News Detection, which contains statements classified into "True" and "False" categories.

### Project Structure

- **DataPrep.py**: Preprocesses and analyzes data, including exploratory data analysis and data quality checks.
- **FeatureSelection.py**: Implements feature extraction and selection methods, including bag-of-words, n-grams, and term frequency weighting.
- **classifier.py**: Builds and evaluates classifiers, including Naive Bayes, Logistic Regression, SVM, Stochastic Gradient Descent, and Random Forest.
- **prediction.py**: Utilizes the final Logistic Regression classifier to predict the class of a news headline provided by the user.

## Performance

Our best-performing model, Logistic Regression, achieved an F1 score in the 70s range. The learning curves illustrate model performance.

## Next Steps

Future improvements could include feature selection techniques like POS tagging, word2vec, and topic modeling, as well as increasing the training data size to enhance model accuracy.

## How to Run the Software

1. Clone this repository to your local machine.
2. Navigate to the project directory.
3. Run the `prediction.py` file as follows:
   - Anaconda: `python prediction.py`
   - Python 3.6: Replace `python` with the full path to your Python executable.

Follow the on-screen instructions to input a news headline and receive the classification and probability of truth.

---

Made By: Shivam Verma
