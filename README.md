# Email / SMS Spam Classification
# Overview
This project focuses on classifying emails and SMS messages into spam and non-spam (ham) categories using machine learning techniques. It involves data cleaning, exploratory data analysis (EDA), data preprocessing, and model building to create an effective spam classifier.

# Project Steps
1. Data Loading
The dataset was obtained from Kaggle and served as the foundation of this project.

3. Data Cleaning
Irrelevant columns were dropped from the dataset, and the remaining columns were renamed for clarity.

Label encoding was applied to the target variable to convert it into numerical values.

Null and duplicated values were checked and handled, with duplicate rows being kept only once.

5. Exploratory Data Analysis (EDA)
The dataset was examined to identify any imbalances between spam and ham categories.

NLTK was imported to perform Natural Language Processing (NLP) tasks.

Additional features such as the number of characters, words, and sentences in each text were extracted.

Tokenization of words and sentences was performed to facilitate analysis.

Differences between spam and ham messages were explored using descriptive statistics.

7. Data Preprocessing
Stopwords were downloaded from the NLTK library and used to filter out common, uninformative words.

Text was converted to lowercase, tokenized, and special characters were removed.

Stemming was applied to ensure uniformity of words.

The preprocessed text was stored in a new feature called "transformed_text."

9. Model Building
TF-IDF (Term Frequency-Inverse Document Frequency) vectorization was applied to convert the transformed text into numerical features.

The dataset was split into training and testing sets.

Various machine learning algorithms, including Naive Bayes, Decision Tree, Random Forest, and Logistic Regression, were implemented.

Naive Bayes demonstrated the highest precision among the models.

11. Important details 
Data Cleaning:
Null values in several columns were identified, and the decision was made to remove columns with a significant number of null values.
Column renaming and label encoding were performed for data clarity and model compatibility.

Tokenization and Text Preprocessing :
Tokenization was achieved using the NLTK library, which split text into words and sentences.
Special characters were removed, and stopwords were filtered out to prepare the text for analysis.

TF-IDF Vectorization :
TF-IDF was selected as it assigns more weight to unique words and less to common words.
This vectorization technique is particularly suitable for text classification tasks.

Model Selection and Evaluation :
Models such as Naive Bayes, Decision Tree, Random Forest, and Logistic Regression were chosen for their ability to handle text data.
Evaluation metrics included accuracy, precision, recall, and F1-score.
Precision was prioritized due to the imbalance in the dataset, focusing on minimizing false positives.

# Challenges
Handling imbalanced data, where ham data outnumbered spam data.

Proper text preprocessing was crucial to ensure high-quality data and model performance.

Feature engineering played a role in improving model performance.

Addressing the challenge of minimizing false positives in a skewed dataset.

# Conclusion
This project successfully demonstrates the classification of emails and SMS messages into spam and ham categories. The use of TF-IDF vectorization and machine learning algorithms like Naive Bayes resulted in an effective spam classifier.
