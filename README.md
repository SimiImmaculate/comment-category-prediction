# Comment Category Prediction

A multiclass text-classification project developed for the **Comment Category Prediction Challenge** on Kaggle.

The project focuses on classifying user comments into four categories using Natural Language Processing (NLP), feature engineering, classical machine learning, LightGBM, and ensemble learning.

## Project Objective

Build a machine learning pipeline capable of predicting the category of a comment from textual and structured features.

The project explores how text representation, feature engineering, model selection, and ensemble methods can be combined to improve multiclass classification performance.

## Dataset

The competition dataset contains:

- Approximately 198,000 training records
- Approximately 102,000 test records
- 4 target classes
- Textual, numerical, categorical, and date-related features

The original Kaggle datasets are **not included in this repository** because they are competition data.

## Project Workflow

```text
Raw Data
    |
    v
Data Inspection
    |
    v
Missing Value Handling
    |
    v
Duplicate Checks
    |
    v
Feature Engineering
    |
    v
Text Preprocessing
    |
    v
TF-IDF Representation
    |
    v
Train / Validation Split
    |
    v
Baseline Models
    |
    v
Model Comparison
    |
    v
Cross-Validation
    |
    v
Hyperparameter Tuning
    |
    v
Ensemble Learning
    |
    v
Final Evaluation
```
## Feature Engineering

The project creates and evaluates several features, including:

- Comment length
- Word count
- Unique-word ratio
- Vote-related features
- Date and time features
- Year
- Month
- Hour
- Text-based TF-IDF features
- Word n-grams
- Character-level features

## NLP Approach

The text classification pipeline uses TF-IDF-based representations to convert comments into numerical features.

Both word-level and character-level text features were explored.

The project also investigates text preprocessing operations such as:

- Lowercasing
- Tokenization
- Stop-word handling
- N-gram generation
- Sparse text representations

## Machine Learning Models

Multiple models were explored during the project, including:

- Logistic Regression
- Linear SVM
- Ridge-based classification
- SGD-based classifiers
- Multinomial Naive Bayes
- Random Forest
- AdaBoost
- MLP
- LightGBM

Model performance was compared using classification metrics appropriate for the multiclass problem.

## Model Optimization

The project includes:

- Cross-validation
- Randomized hyperparameter search
- Feature engineering experiments
- Model comparison
- Ensemble learning

The final modelling workflow combines **Logistic Regression and LightGBM through voting ensemble learning**.

## Result

The submitted solution achieved a **0.83016 Kaggle competition score**.

The validation experiments also used **Macro-F1** to evaluate performance across the four classes.

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- LightGBM
- Matplotlib
- Seaborn
- Jupyter Notebook
- Kaggle

## Repository Structure

```text
comment-category-prediction/
|
|-- comment-category-prediction.ipynb
|-- .gitignore
`-- README.md
```
## Key Learning Outcomes

Through this project, I worked with:

- Multiclass classification
- Natural Language Processing
- TF-IDF feature engineering
- Sparse feature representations
- Structured and text feature integration
- Model comparison
- Cross-validation
- Hyperparameter tuning
- Ensemble learning
- Kaggle-based machine learning workflow

## Data and Reproducibility

The original competition datasets are intentionally excluded from this repository.

The notebook contains the analysis and modelling workflow used during the project. Dataset paths may need to be updated when reproducing the work with the competition data.

## Author

**Simi Immaculate**

M.Sc. Mathematics | Data Science & Machine Learning

GitHub: [SimiImmaculate](https://github.com/SimiImmaculate)
