# Steam Review Sentiment Analysis

## Project Overview

This project applies machine learning and Natural Language Processing (NLP) techniques to analyse player sentiment from Steam game reviews.

The objective is to classify reviews as positive or negative and provide business insights for game developers regarding player satisfaction.

## Dataset

* Source: Public Steam Reviews Dataset
* Original Size: 6,417,106 reviews
* Sample Used: 50,000 reviews
* Final Cleaned Dataset: 41,319 reviews

Features:

* app_id
* app_name
* review_text
* review_score
* review_votes

## Methods Used

### Data Preprocessing

* Missing value removal
* Duplicate removal
* Text cleaning
* Lowercasing
* URL removal
* Punctuation removal
* TF-IDF vectorisation

### Machine Learning Models

* Naive Bayes
* Logistic Regression
* Linear Support Vector Machine (SVM)

## Results

| Model               | Accuracy |
| ------------------- | -------- |
| Naive Bayes         | 85.20%   |
| Logistic Regression | 87.55%   |
| Linear SVM          | 87.54%   |

Final selected model: **Linear SVM**

Reason:
Although Logistic Regression achieved slightly higher accuracy, Linear SVM performed better at detecting negative reviews, which was more valuable for the business problem.

## Business Value

This system can help game developers:

* Monitor player satisfaction
* Detect negative sentiment after updates
* Identify issues such as bugs, crashes, and balancing problems
* Improve decision-making using player feedback

## Technologies

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Jupyter Notebook
