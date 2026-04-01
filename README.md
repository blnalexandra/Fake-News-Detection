# Fake News Classification
ML project that classifies news articles as real or fake using simple classsification models and NLP techniques.

## Data Cleaning
- Removed unnecessary column (Unnamed: 0)
- Handled missing values
- Combined title + text into a single column (content)
- Shuffled dataset for randomness

## Text Cleaning
- Created a custom clean_text() function that does: lowercase, removes URLs, HTML tags, punctuation, numbers and removes english stopwords using sklearn

## Feature Engineering
- Used TF-IDF Vectorization
- Limited to 5000 features to keep model efficient

## Train-Test Split
- 80/20 split

## Models Used
### Logistic Regression:
-  Works well for text classification problems
-  Accuracy: 95%
-  Balanced precision and recall
### Linear SVM:
- Very effective for high-dimensional data like TF-IDF
- Accuracy: 95%
- Slightly better recall for fake news

## Conclusion
- Could use hyperparameter tuning
- More advanced text preprocessing
- Strong results from both models but SVM has a slight margin over LR
- Over 90% accuracy even without deep learning or a lot of tuning
