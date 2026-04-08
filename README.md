# Understanding the Importance of Calibrating Machine Learning Models

<p>
  <img alt="ML Model Reliability/Calibration figure" src="imgs/"/>
</p>

[img source: ](url)

## Project Description

This project emphasizes the need for data and machine learning scientists to calibrate their machine learning classification models<sup>\*</sup>. Here, model calibration relates to the process of adjusting a classifier so that its predicted probability (e.g., 80%) actually reflects the true frequency of the event occurring in the real world (e.g., 8 out of 10 people). It ensures that a model's "confidence" matches its actual accuracy, transforming raw scores into reliable risk estimates. This project show you how to test for calibration, how to calibrate a learning model, and most importantly how to use a calibrated model afterwards.

The project relies on the heart disease dataset, a reliable and extensivley used resource in cardiovascular research medical studies, and machine learning applications. While the original dataset has 76 attributes or features, the dataset used here only uses 14 crucial features linked to heart disease diagnosis. The **target** or prediction is a binary classification indicating whether a patient has heart disease (target = 1) or not (target = 0).

<sup>\*</sup> Calibration applies to regression models as well, but the concept of predicting probabilities as in classification shifts to predcting uncertainty and intervals. In these situations, a calbibrated model is one where the predicted uncertainty (like a variance or confidence interval) accurately reflects the actual distribution of the data.
This project reveals calibration for classification models solely.

### The Problem

** Raw accuracy (i.e., taking the probabilities from an uncalibrated classification model) is not enough.**

Especially considering the high-stakes decisions of making a diagnosis of heart disease or not. While a standard machine learning model might correctly identify a patient at risk, its predicted probability (e.g., 0.8) often doesn't reflect the real-world likelihood of the disease.

In this project using the UCI Heart Disease dataset, I found that models like Radom Forests, Naive Bayes, or SVMs can be "overconfident" or "underconfident." Calibration ensures that if the model predicts a 80% chance of heart disease, roughly 80% of those patients actually have the condition.

Without calibration, a doctor might misinterpret a "risk score" as a simple binary flag, leading to unnecessary invasive procedures or, worse, missed diagnoses. The whole point is to align predicted probabilities with clinical reality --think, transforming a black-box algorithm into a reliable diagnostic tool that supports precise, risk-adjusted medical interventions.

### What this Project Does Specifically

The project:

- Loads and inspects the banking data
- Preprocesses/cleans the data
- Performs exploratory data analysis (EDA)
  - Statistical summary of the data
  - Normalize the data
  - Feature engineering
    - Categorical encoding
  - Univariate analysis
  - Bivariate analysis
- Tests for balanced and imbalanced data sets
- Calibrates different types of Machine Learning models to show the importance of Calibration

### Summary, Actionable Insights, and Business Recommendations

---

## Objective

The project contains the key elements:

- `Git` (version control),
- `Jupyter` Python coded notebooks,
- `Matplotlib` visualization of data,
- `Numpy` for arrays and numerical operations,
- `Pandas` for dataframe usage,
- `Python` the standard modules,
- `Seaborn` visualization of data,
- `Scikit-Learn` to get training and test datasets,
- `uv` package management including use of `ruff` for linting and formatting

## Tech Stack

![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-%23121011.svg?logo=github&logoColor=white)
![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)
![Matplotlib](https://custom-icon-badges.demolab.com/badge/Matplotlib-71D291?logo=matplotlib&logoColor=fff)
![Numpy](https://img.shields.io/badge/Numpy-777BB4?style=for-the-badge&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?logo=pandas&logoColor=fff)
![Plotly](https://img.shields.io/badge/Plotly-239120?style=for-the-badge&logo=plotly&logoColor=white)
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Scikit-Learn](https://img.shields.io/badge/scikit_learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white)

---

## Getting Started

Here are some instructions to help you set up this project locally.

---

## Installation Steps

The Python version used for this project is `Python 3.12 or higher` to be compatible with TensorFlow.

Follow the requirements for using TensorFlow [here](https://www.tensorflow.org/install/pip#macos)

use `uv pip install tensorflow`

- Make sure to use python versions `Python 3.9–3.12
- pip version 19.0 or higher for Linux (requires manylinux2014 support) and Windows. pip version 20.3 or higher for macOS.
- Windows Native Requires Microsoft Visual C++ Redistributable for Visual Studio 2015, 2017 and 2019

### Clone the Repo

1. Clone the repo (or download it as a zip file):

   ```bash
   git clone https://github.com/beenlanced/ml_mentoring_model_calibration_problem.git
   ```

2. Create a virtual environment named `.venv` using `uv` Python version 3.11:

   ```bash
   uv venv --python=3.12
   ```

3. Activate the virtual environment: `.venv`

   On macOS and Linux:

   ```bash
   source .venv/bin/activate #mac
   ```

   On Windows:

   ```bash
    # In cmd.exe
    venv\Scripts\activate.bat
   ```

4. Install packages using `pyproject.toml` or (see special notes section)

   ```bash
   uv pip install -r pyproject.toml
   ```

### View Notebooks to see Exploratory Data Analysis and Predicative Model Construction

---

## Dataset

We use open-source datasets from Kaggle: []().

The dataset contains 10,000 sample points with 14 distinct features such as

---

### Final Words

Thanks for visiting.

Give the project a star (⭐) if you liked it or if it was helpful to you!

You've `beenlanced`! 😉

---

## Acknowledgements

I would like to extend my gratitude to all the individuals and organizations who helped in the development and success of this project. Your support, whether through contributions, inspiration, or encouragement, have been invaluable. Thank you.

Specifically, I would like to acknowledge:

- The folks who host the []().
- The UCI ECG heartbeat heart disease categorization/classification dataset found [on Kaggle](https://www.kaggle.com/datasets/zhaoyingzhu/heartcsv/data).

- Guidance from [](https://github.com/ritvikmath/YouTubeVideoCode/blob/main/Probability%20Calibration.ipynb).

- [](https://www.kaggle.com/code/abolfazluk/ai-powered-heart-health-prediction-uci-dataset/notebook)

- [Hema Kalyan Murapaka](https://www.linkedin.com/in/hemakalyan) and [Benito Martin](https://martindatasol.com/blog) for sharing their README.md templates upon which I have derived my README.md.

- The folks at Astral for their UV [documentation](https://docs.astral.sh/uv/)

---

## License

This project is licensed under the MIT License - see the [LICENSE](./LICENSE) file for details
