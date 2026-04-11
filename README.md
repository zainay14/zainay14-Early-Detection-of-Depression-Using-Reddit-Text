# Early Depression Detection
Mental health issues, especially depression, are becoming increasingly prevalent in today’s digital world. Many individuals express their emotions and struggles through social media platforms like Reddit. Early identification of depressive behavior can help in timely intervention and support. This project focuses on detecting depression from textual data using machine learning techniques to improve mental health awareness and support systems.
The objective of this study is to classify whether a given Reddit post indicates depression or not. The dataset originally contains multiple mental health categories such as Depression, Anxiety, Bipolar, and Suicidal. For simplicity and practical implementation, the problem is converted into a binary classification task:

- 1 → Depression
- 0 → Other mental health conditions

To solve this problem, multiple machine learning models are implemented and compared, including Logistic Regression, Support Vector Machine (SVM), Naive Bayes, and Random Forest. Text data is preprocessed and transformed into numerical features using TF-IDF vectorization.
The results show that although models achieve high accuracy, performance is affected by class imbalance. Among all models, SVM and Logistic Regression provide a relatively better balance between precision and recall.

## Instructions
The project is implemented in Python using Jupyter Notebook.
You can run the notebook:
 - On Google Colab, or
 - Locally using Jupyter Notebook / JupyterLab

## Dataset
- The dataset contains Reddit posts labeled with different mental health conditions.
- File used: [link Text](Sentiment_Mental_health_dataset.xls)
- Total records: 26,350 entries
- Features:
    - statement → Text data (Reddit post)
    - status → Mental health category
## Project Workflow
#### 1. Data Loading
- Load dataset using Pandas
#### 2. Data Preprocessing
- Convert text to lowercase
- Handle categorical labels
- Convert multi-class labels into binary labels
#### 3. Exploratory Data Analysis (EDA)
- Analyze class distribution
- Identify dataset imbalance
#### 4. Feature Engineering
- Apply TF-IDF Vectorization
- Use unigrams and bigrams (n-grams)
- Limit features to top 8000
#### 5. Train-Test Split
- 80% training, 20% testing
- Stratified sampling to preserve class distribution
#### 6. Model Implementation
- Logistic Regression
- Support Vector Machine (SVM)
- Naive Bayes
- Random Forest
#### 7. Model Evaluation
- Accuracy
- Precision
- Recall
- F1 Score
- Log Loss

## Results Summary
#### 1. Logistic Regression
- Good overall accuracy
- Low recall due to imbalance
#### 2. SVM
- Better balance between precision and recall
- Performs relatively well for this task
#### 3. Naive Bayes
- Fast but poor recall performance
#### 4. Random Forest
- High precision
- Very low recall (misses many depression cases)

## Conclusion

This project demonstrates how Natural Language Processing (NLP) and machine learning can be used for early detection of depression from social media text. While traditional models show promising results, class imbalance significantly impacts performance.
Confusion Matrix
