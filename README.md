# DeGatto: A Sentiment Analysis Framework for E-Commerce

## Authors
Aine Drelingyte, Axelle Gapin, Omar AbedelKader, Danyl Shkrebko, Elie Dina, Joseph Jreije, Quentin Herbin

## Institution
Université de Lorraine, IDMC

## Abstract
Sentiment Analysis (SA) identifies and categorizes views expressed in text. The "DeGatto" project focuses on SA in women's apparel marketing by analyzing an e-commerce corpus at the sentence and aspect levels, applying various Natural Language Processing (NLP), Deep Learning (DL), and Machine Learning (ML) models. The project's objective is to select suitable models and hyperparameters for accurate sentiment analysis.

## Introduction
SA has become a significant research topic in domains like business and politics. This project aims to analyze women's apparel reviews using sentence-level and aspect-level analysis to determine the best-performing models and hyperparameters.

## Background
### Process of Sentiment Analysis
The SA process involves:
1. Data collection
2. Text pre-processing
3. Sentiment detection
4. Sentiment classification
5. Output presentation

### Sentiment Classification
SA can be performed at different levels:
- **Document-level**: Provides overall sentiment.
- **Sentence-level**: Analyzes sentiment per sentence.
- **Aspect-level**: Identifies polarity based on specific targets.

## Project "DeGatto"
### Overview
The "DeGatto" project adapts SA to women’s apparel reviews, aiming to support e-commerce companies and customers by providing feedback analysis on aspects like material, size, design, and comfort.

### Data
The data is sourced from Kaggle and includes:
- Women’s clothing reviews
- 23,000 sentences and 251,000 tokens
- Key attributes: clothing ID, recommendation score, review text, rating

The final annotated corpus consists of 23,562 sentences with aspect-level labels for comfort, longevity, size, design, and material.

### Visualization Tool
A web-based tool was developed for data visualization using:
- **Front-end**: ReactJS
- **Back-end**: NodeJS
- Graph options: Bar chart, pie chart
- Analyses: Sentence-level, aspect-level

### Text Preprocessing and Annotation
Text data is cleaned by removing punctuation, duplicates, and manually selected stop-words. The data is manually annotated to achieve high accuracy, with the process validated using Cohen’s kappa coefficient for inter-annotator agreement.

## NLP Models and Methods
The following models were evaluated:
- **LSTM (BiLSTM)**: Performs best in sentence-level analysis.
- **Support Vector Machine (SVM)**
- **Logistic Regression (LR)**
- **Multinomial Naive Bayes (MNB)**

Hyperparameters like alpha (MNB), C-value, max iterations (SVM, LR), and epochs (BiLSTM) were tuned to enhance performance.

## Results and Discussion
The models were tested on both sentence-level and aspect-level datasets:
- **Sentence-level**: BiLSTM achieved the highest accuracy (94%).
- **Aspect-level**: LinearSVC performed well, particularly for size and material aspects.

### Performance Observations
- BiLSTM: Best results in sentence-level and design aspect-level analyses.
- MNB: Underperformed in all analyses, likely due to its assumption of feature independence.

## Conclusion
The project effectively identified suitable models and hyperparameters for accurate sentiment analysis in women's apparel reviews. The BiLSTM model was the best performer for sentence-level analysis, while LinearSVC excelled at aspect-level sentiment analysis.

## References
- Key papers on SA techniques, model comparisons, and recent advancements in NLP and DL models.
