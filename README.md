# 🧠 Mental Health Data Analysis

**Exploratory analysis and statistical investigation of factors associated with mental-health indicators**

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sadiashatabdi/Mental-Health-/blob/main/mental_health.ipynb)
[![Python](https://img.shields.io/badge/Python-3.12+-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data_Analysis-150458?logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Scikit-Learn](https://img.shields.io/badge/scikit--learn-Machine_Learning-F7931E?logo=scikitlearn&logoColor=white)](https://scikit-learn.org/)

---

## 📌 Overview

This project presents an exploratory and statistical analysis of survey data related to mental-health indicators. The notebook examines demographic, lifestyle, behavioral, and psychological variables, including stress, mood swings, coping difficulties, indoor activity, work interest, and social weakness.

The analysis combines:

- Exploratory data analysis
- Missing-value and data-quality checks
- Categorical data visualization
- ANOVA and hypothesis testing
- Machine-learning preprocessing and experimentation
- Pattern identification across mental-health-related variables

> **Disclaimer:** This repository is intended for educational and research purposes only. It does not provide medical advice, diagnosis, or treatment recommendations.

---

## 📊 Dataset

The notebook uses `mental_health_finaldata_1.csv`, containing **824 records and 13 variables**.

| Variable | Description |
|---|---|
| Age | Age group of the participant |
| Gender | Gender category |
| Occupation | Occupation or employment category |
| Days_Indoors | Time spent indoors |
| Growing_Stress | Reported increase in stress |
| Quarantine_Frustrations | Frustration experienced during quarantine |
| Changes_Habits | Reported changes in habits |
| Mental_Health_History | Previous or existing mental-health history |
| Weight_Change | Reported change in weight |
| Mood_Swings | Frequency or severity of mood swings |
| Coping_Struggles | Difficulty managing stress or difficult situations |
| Work_Interest | Reported interest in work |
| Social_Weakness | Social withdrawal or social weakness indicator |

The notebook reports **no missing values** across the 13 variables.

> The dataset may contain self-reported information. Ensure that any dataset license or source terms are respected before reuse.

---

## 🔬 Methodology

```text
Dataset Loading
      ↓
Data Validation and Cleaning
      ↓
Exploratory Data Analysis
      ↓
Categorical Distribution Visualization
      ↓
Statistical Hypothesis Testing
      ↓
Categorical Variable Processing
      ↓
Machine-Learning Analysis
```

### 1. Data Quality and Preprocessing

The notebook:

- Loads the dataset with Pandas
- Inspects column types and dataset dimensions
- Checks for missing values
- Examines the number of unique values in each column
- Converts selected categorical variables into numerical representations

### 2. Exploratory Data Analysis

The visualization workflow includes:

- Count plots for categorical variables
- Distribution plots for the first and final columns in the dataset
- Missing-value heatmaps
- Descriptive summaries for categorical fields

### 3. Statistical Analysis

The notebook formulates and evaluates hypotheses related to:

- Days spent indoors and growing stress
- Days spent indoors and mood swings
- Quarantine frustration and quarantine-related negative impact
- Mental-health history and quarantine-related negative impact
- Mental-health history and work interest

Statistical methods include:

- ANOVA
- Chi-square testing
- Correlation analysis

## 🤖 Machine-Learning Workflow

The notebook imports `RandomForestClassifier` and scikit-learn utilities for classification experimentation.

A typical supervised-learning pipeline includes:

1. Encoding categorical variables
2. Separating features and target variables
3. Splitting the data into training and testing sets
4. Training a machine-learning model
5. Evaluating predictions
6. Examining feature importance or model behavior

Model results should be interpreted with appropriate caution, especially because survey responses may be subjective and the dataset may not represent the general population.

---

## 🚀 Getting Started

### Run in Google Colab

1. Click the **Open in Colab** badge above.
2. Upload `mental_health_finaldata_1.csv` to the Colab session.
3. Update the CSV path if necessary:

```python
dataset = pd.read_csv("/content/mental_health_finaldata_1.csv")
dataset.head()
```

4. Run all notebook cells from **Runtime → Run all**.

### Run Locally

```bash
git clone https://github.com/sadiashatabdi/Mental-Health-.git
cd Mental-Health-

python -m venv .venv
source .venv/bin/activate

pip install pandas numpy matplotlib seaborn scipy scikit-learn
jupyter notebook mental_health.ipynb
```

On Windows, activate the environment with:

```bash
.venv\Scripts\activate
```

---

## 📦 Requirements

The notebook uses:

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- Scikit-learn
- SQLite
- gdown

You may install the main Python packages with:

```bash
pip install pandas numpy matplotlib seaborn scipy scikit-learn gdown
```

---

## 📁 Repository Structure

```text
Mental-Health-/
├── mental_health.ipynb
└── README.md
```

---

## ⚠️ Limitations

- Survey responses may contain subjective or self-reporting bias.
- Categorical variables require appropriate encoding and validation.
- Statistical associations do not necessarily represent causal relationships.
- Findings may not generalize to broader or clinical populations.
- The project should not be used for diagnosis, treatment, or clinical decision-making.

---

## 🔮 Future Work

- Add complete train-test and cross-validation metrics
- Compare multiple classification algorithms
- Evaluate model performance using multiple metrics
- Perform additional feature-selection and feature-engineering analysis
- Incorporate explainable-AI methods
- Include model and analysis visualizations
- Validate findings using a larger and more representative dataset
- Develop an interactive data-visualization dashboard

---

## 👩‍💻 Author

**Sadia Shatabdi**

GitHub: [@sadiashatabdi](https://github.com/sadiashatabdi)

---

<div align="center">

If you find this project useful, please consider giving it a ⭐.

</div>
