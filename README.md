# EECE_490_Hackathon

# Big Five Personality Traits and Behavioral Analysis

This project explores the relationships between the Big Five personality traits and various behavioral and demographic attributes. Using machine learning models, we predict outcomes such as exercise habits, social media usage, stress levels, and more.

## Table of Contents
1. [Introduction](#introduction)
2. [Project Workflow](#project-workflow)
   - [Data Preprocessing](#data-preprocessing)
   - [Correlation Analysis](#correlation-analysis)
   - [Model Training](#model-training)
   - [Evaluation](#evaluation)
3. [Results and Visualizations](#results-and-visualizations)
4. [How to Run the Code](#how-to-run-the-code)
5. [Dependencies](#dependencies)
6. [Acknowledgements](#acknowledgements)

---

## Introduction

This project uses a dataset with responses to personality and behavioral surveys. The main goals are:
- To compute Big Five personality scores: Extraversion, Agreeableness, Conscientiousness, Neuroticism, and Openness.
- To understand correlations between personality traits and outcomes such as smoking habits, social media usage, and financial behavior.
- To train models to predict key behavioral patterns and demographics based on personality traits.

---

## Project Workflow

### 1. Data Preprocessing
- **Column Renaming**: The dataset's columns were renamed for clarity using a mapping dictionary.
- **Value Mapping**: Categorical values (e.g., "Agree strongly") were converted to numerical scales.
- **Handling Missing Data**: Missing values were identified and addressed.

### 2. Correlation Analysis
- Identified features correlated with each target variable.
- Used these correlated features to enrich the predictive power of the models.

### 3. Model Training
- Used the following models:
  - **Random Forest Classifier** for categorical predictions (e.g., exercise rate, stress frequency).
  - **Random Forest Regressor** for continuous predictions (e.g., first cigarette age).
- Split data into training and testing sets (70-30 split).

### 4. Evaluation
- **Classification**: Metrics such as accuracy, precision, recall, and F1-score were used.
- **Regression**: Mean Squared Error (MSE) was calculated.

---

## Results and Visualizations

The following are key results from the analysis:
- **Accuracy Scores**: 
  - Exercise Rate: 38%
  - Social Media Time: 44%
  - Stress Frequency: 42%
  - Employment Status: 72%
  - Income Sufficiency: 31%

- **Best Performing Models**: 
  - Predicting "Switching Cigarette Brand Due to Crisis" (91% accuracy).
  - Predicting "Close Friends" status (98% accuracy).

### Visualization
Generated bar plots to illustrate model accuracies:
- **Model Accuracy by Target Variable**: A horizontal bar chart shows performance for each target.

---

## How to Run the Code

1. Clone this repository or download the notebook.
2. Install the required dependencies listed below.
3. Run the notebook in any Python environment (e.g., Jupyter, Google Colab).
4. Follow the steps in the notebook:
   - Upload the dataset.
   - Execute preprocessing and correlation steps.
   - Train and evaluate models.
   - View results and visualizations.

---

## Dependencies

The project requires the following Python libraries:
- `pandas`
- `numpy`
- `matplotlib`
- `scikit-learn`

Install dependencies with:
```bash
pip install pandas numpy matplotlib scikit-learn
