# Product-Review-Analysis
#### Overview
This project involves analyzing the Amazon Alexa dataset and building classification models to predict whether the sentiment of a given input sentence is positive or negative.

#### Steps Involved

1. **Importing Required Libraries**
    - Libraries such as NumPy, Pandas, Matplotlib, Seaborn, and NLTK were imported for data manipulation, visualization, and natural language processing tasks.

2. **Exploratory Data Analysis (EDA)**
    - The dataset was loaded and initial exploration was performed to understand its structure and contents.
    - Columns were examined for null values, and a record with a missing 'verified_reviews' field was identified and dropped.
    - A new column named 'length' was created to store the length of the reviews.

3. **Data Preprocessing**
    - Reviews were tokenized, and stop words were removed using NLTK.
    - Text stemming was performed using the PorterStemmer from NLTK.
    - The processed text was converted into numerical features using CountVectorizer and TF-IDF Vectorizer.

4. **Model Building and Evaluation**
    - Several machine learning models were built and evaluated, including:
        - Logistic Regression
        - Random Forest Classifier
        - XGBoost Classifier
        - Decision Tree Classifier
    - For each model:
        - Cross-validation and grid search were performed to find the best hyperparameters.
        - Training and testing accuracies were calculated.
        - Confusion matrices were generated to visualize model performance.
    - The XGBoost model was saved using pickle for future use.

5. **Visualization**
    - Various visualizations were created to aid in understanding data distribution and model performance, such as confusion matrices and other relevant plots.

#### Key Findings
- The models built provided insights into the sentiment analysis of Amazon Alexa reviews.
- XGBoost Classifier showed strong performance and was saved for future predictions.
