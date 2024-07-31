# Questionpaper_Difficulty_Analysis
## Project Overview

Implemented Python programming in Jupyter Notebook to deploy algorithms for data preprocessing on question data, partitioning it into training and test sets for further analysis. Utilized machine learning methods to analyze student feedback and categorize question paper difficulty, aiding in a deeper comprehension of test perception and assessment methodologies. Visualized and compared model accuracies, highlighting the Random Forest classifier's performance at 94.6% accuracy.

### Main Objective

The main objective of this project is to understand and categorize the perceived difficulty of questions based on student feedback, thereby improving test assessment methodologies. We aim to understand how students feel about the difficulty of their exam questions by analyzing their feedback. By using machine learning techniques, we can classify and understand these perceptions better. This helps in improving how exams are created and assessed, making the evaluation process more effective and fairer for students.

### Brief Description

We leveraged student feedback from survey comments to assess the difficulty level of question papers, categorizing them as "easy," "medium," or "hard." Using data from Kaggle, we implemented Naive Bayes, Decision Tree, and Random Forest classifiers to analyze and classify these perceptions. The extracted sentiments from numerous students formed decision attributes for our models, enabling a detailed analysis of question paper difficulty.

## Dataset Description & Sample Data

The dataset (`predictiondata.csv`) which we are using contains 530 records, in which each record contains:
1. **CGPA** classified as "Above average," "Average," and "Below average"
2. **Difficulty levels for five questions** given as easy, medium, and hard.
3. **Overall Difficulty level** (EASY, MEDIUM, TOUGH) as the target attribute.

[Dataset Link Analysis of Question Paper (Kaggle)](https://www.kaggle.com/)

## Tools Used

- Jupyter Notebook

## Project Modules

1. **CGPA Classification ("Above average," "Average," "Below average")**:
   - Provides a broad indicator of a student's academic performance, helping to correlate their perception of question difficulty.

2. **Difficulty Levels for Five Questions (Easy, Medium, Hard)**:
   - Enables detailed analysis of individual question challenges, aiding in targeted improvements in exam design.

3. **Overall Difficulty Level (Easy, Medium, Tough) as the Target Attribute**:
   - Provides a comprehensive view of the exam's perceived difficulty, serving as the target for classification and prediction in the analysis.

## Models Used

- **Random Forest**
- **Naive Bayes**
- **Decision Tree**

We found that the Random Forest algorithm has the highest accuracy among all the algorithms.

## Advantages

- **Improved Understanding of Student Perceptions**: Provides detailed insights into how students perceive the difficulty of exam questions, helping educators identify areas where students may struggle.
- **Data-Driven Decision Making**: Utilizes machine learning techniques to objectively analyze feedback, leading to a more accurate and reliable assessment of question difficulty.
- **Enhanced Assessment Methodologies**: Helps in refining and improving the way exams are structured and assessed, ensuring they are fair and appropriately challenging for students.
- **Personalized Learning**: Enables educators to tailor their teaching strategies based on the identified difficulty levels, addressing individual student needs more effectively.
- **Resource Optimization**: Assists in better resource allocation by identifying which topics or types of questions require more focus and improvement.
- **Scalability**: The framework can be applied to various educational settings and different types of exams, making it a versatile tool for continuous improvement in education.

## Proposed Algorithm with Flowchart

### Data Collection
- The initial step involves collecting data on the question paper, including the number of questions in it. Both human and automated methods can be used to obtain this data.

### Pre-processing
- Necessary to get rid of any redundant or irrelevant information after the data has been acquired. Steps include data cleaning, standardization, and transformation.

### Feature Extraction
- The pre-processed data is used to feature extraction, choosing the pertinent data and turning it into an analytically-ready numerical representation of the questions' level of difficulty.

### Test Split
- The data can be split into two sets, a training set and a testing set. The model is trained on the training set, and the testing set is used to evaluate the model's performance.

### Machine Learning Models
- These models examine the extracted features to ascertain the degree of difficulty of the exam questions. Depending on the availability of labeled data, the models can be trained using supervised or unsupervised learning techniques.

### Model Training
- Once the model is selected, it needs to be trained on the pre-processed data. The data is split into training and validation sets to evaluate the model's performance.

### Analysis
- The machine learning models' analysis is used to assess the question paper's level of difficulty. The quality of upcoming question papers can be improved by using this information to pinpoint the topics that caused pupils the most difficulty.

### Visualization
- Lastly, graphs, charts, or other visual aids might be used to illustrate the study findings. This makes the information easier to acquire and comprehend.

## Random Forest

- Random Forest is a popular machine learning algorithm that belongs to the supervised learning technique. It can be used for both Classification and Regression problems in ML.
- It is a classifier that contains a number of decision trees on various subsets of the given dataset and takes the average to improve the predictive accuracy of that dataset.
- It is based on the concept of ensemble learning, which is a process of combining multiple classifiers to solve a complex problem and to improve the model's performance.
- The greater number of trees in the forest leads to higher accuracy and prevents the problem of overfitting.

## Decision Tree

- Decision Tree is a Supervised learning technique that can be used for both classification and Regression problems. It is a tree-structured classifier where internal nodes represent the features of a dataset, branches represent the decision rules, and each leaf node represents the outcome.
- It is a graphical representation for getting all the possible solutions to a problem/decision based on given conditions.

## Naive Bayes

- Naïve Bayes algorithm is a supervised learning algorithm based on Bayes theorem and used for solving classification problems. It is mainly used in text classification that includes a high-dimensional training dataset.
- Naïve Bayes Classifier is one of the simple and most effective Classification algorithms which helps in building fast machine learning models that can make quick predictions. It is a probabilistic classifier, which means it predicts on the basis of the probability of an object.

## Challenges and Solutions

1. **Data Collection and Preprocessing**
   - **Challenge**: The raw data from Kaggle consisted of unstructured student comments, which were often noisy and contained irrelevant information.
   - **Solution**: Applied text preprocessing techniques like removing punctuation, stopwords, special characters, tokenization, and lemmatization.

2. **Imbalanced Data**
   - **Challenge**: The dataset was imbalanced, with significantly more comments in some categories compared to others.
   - **Solution**: Employed resampling techniques like oversampling for minority classes and undersampling for majority classes. Used SMOTE to generate synthetic samples for the underrepresented classes.

3. **Model Selection and Tuning**
   - **Challenge**: Selecting the right machine learning models and tuning their hyperparameters.
   - **Solution**: Implemented and compared multiple models.
