# 🇿🇦 South African Job Market Intelligence & ML

## 📌 Project Overview

This project analyses South African job-market listings to identify employment trends, in-demand technical skills, job characteristics, and patterns within technology-related roles.

The project combines **data analysis, exploratory data analysis (EDA), Natural Language Processing (NLP), feature engineering, and machine learning** to analyse job descriptions and classify technology-related job postings.

---

## 🎯 Objectives

The main objectives of this project are to:

* Explore South African job-market listings.
* Analyse job categories and locations.
* Investigate seniority and remote-work patterns.
* Identify frequently mentioned technical skills.
* Analyse job-description characteristics.
* Apply Natural Language Processing to job descriptions.
* Convert text into numerical features using TF-IDF.
* Train machine-learning classification models.
* Compare Logistic Regression and Random Forest.
* Tune models using GridSearchCV.
* Evaluate model performance using classification metrics.
* Create a function that can classify new job descriptions.

---

## 📊 Dataset

The dataset was collected from the **Job Opportunities API** and contains South African job listings.

The project currently uses a sample of **10 job listings**.

Each listing contains information such as:

* Job title
* Company
* Category
* Location
* Remote-work information
* Seniority
* Posting date
* Employment type
* Job description
* Description length

> **Important:** Because the dataset contains only 10 listings, the findings should not be considered representative of the entire South African job market. The machine-learning results should also be interpreted cautiously.

---

## 🧹 Data Preparation

The data-processing stage included:

* Handling missing categorical values.
* Removing unnecessary columns.
* Converting date fields.
* Creating date-based features.
* Cleaning job descriptions.
* Calculating word and character counts.
* Preparing text for NLP analysis.

---

## 🔎 Exploratory Data Analysis

The project explores several characteristics of the collected job listings, including:

* Job-category distribution
* Location distribution
* Seniority levels
* Remote-work availability
* Job-description length
* Technical-skill frequency

Visualisations were created using **Matplotlib** and **Pandas**.

---

## 💻 Technical Skills Analysis

A predefined list of common technical skills was searched for within job descriptions.

The analysis includes technologies and skills such as:

* Python
* SQL
* R
* Java
* JavaScript
* C++
* C#
* AWS
* Azure
* Google Cloud
* Docker
* Kubernetes
* Git
* GitHub
* Power BI
* Tableau
* Excel
* TensorFlow
* PyTorch
* Scikit-learn
* Pandas
* NumPy
* Machine Learning
* Deep Learning
* Artificial Intelligence
* Data Science
* NLP
* APIs
* Agile
* Scrum

Skill-indicator features were also created for use in further analysis.

---

## 🧠 Natural Language Processing

Natural Language Processing was applied to the job descriptions.

The process included:

1. Converting text to lowercase.
2. Removing HTML.
3. Removing URLs.
4. Removing unnecessary characters.
5. Removing extra whitespace.
6. Creating TF-IDF features.

### TF-IDF

**Term Frequency-Inverse Document Frequency (TF-IDF)** was used to convert job descriptions into numerical features that can be used by machine-learning algorithms.

---

## 🤖 Machine Learning

The project classifies job listings as either:

* **Technology-related**
* **Non-technology-related**

The target variable is:

```text
is_technology_job
```

### Models

Two classification algorithms were implemented:

* Logistic Regression
* Random Forest

### Model Evaluation

The models were evaluated using:

* Accuracy
* Precision
* Recall
* F1-score
* Confusion matrix

---

## ⚙️ Hyperparameter Tuning

`GridSearchCV` was used to search for suitable hyperparameter combinations for the classification models.

The tuned models were then evaluated on the test dataset.

---

## 🔮 Job Description Prediction

A prediction function was developed that allows a new job description to be entered and classified as either a technology-related or non-technology-related job.

Example:

```python
prediction = predict_job_type("""
We are looking for a Python developer with experience
in SQL, APIs, machine learning and cloud technologies.
""")

print(prediction)
```

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Joblib
* Regular Expressions
* Google Colab
* GitHub
* Job Opportunities API

---

## 📁 Project Files

```text
south-african-job-market-ml/
│
├── South_African_Job_Market_Intelligence_ML.ipynb
├── final_south_african_jobs_dataset.csv
├── model_comparison_results.csv
├── south_african_job_classifier.pkl
├── job_description_tfidf_vectorizer.pkl
└── README.md
```

---

## 📈 Project Workflow

```text
Data Collection
       ↓
Data Cleaning
       ↓
Feature Engineering
       ↓
Exploratory Data Analysis
       ↓
Technical Skills Analysis
       ↓
NLP Text Cleaning
       ↓
TF-IDF Feature Extraction
       ↓
Target Creation
       ↓
Train/Test Split
       ↓
Machine Learning
       ↓
GridSearchCV
       ↓
Model Evaluation
       ↓
Prediction
```

---

## ⚠️ Limitations

This project has several limitations:

* The dataset contains only 10 job listings.
* The sample is not representative of the entire South African job market.
* Technical skills were identified using a predefined keyword list.
* Skills outside the predefined list may not have been detected.
* The technology-job target was created using keyword-based rules.
* The small dataset limits the reliability of machine-learning performance measurements.
* Job-market trends change over time.

---

## 🚀 Future Improvements

Future versions could:

* Collect a much larger number of job listings.
* Include multiple job sources.
* Collect listings over a longer period.
* Expand the technical-skills dictionary.
* Apply more advanced NLP techniques.
* Experiment with additional machine-learning algorithms.
* Build an interactive dashboard.
* Regularly update the dataset.
* Track changes in demand for specific technologies over time.

---

## 👩‍💻 Author

**Nobuhle Dhlamini**

Data Science Project — South African Job Market Intelligence & ML

---

## 📜 Project Status

**Completed — Data Science Capstone Project**

