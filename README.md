# Financial-sentiment-analysis

A radial basis support vector classifier based model that analyses reviews and classifies them according to the user sentiment with a precision metric of 83.2%.
The following data is intended for advancing financial sentiment analysis research. It's two datasets (FiQA, Financial PhraseBank) combined into one easy-to-use CSV file. It provides financial sentences with sentiment labels.
API Link : kaggle datasets download -d sbhatti/financial-sentiment-analysis

Prediction model for sentiment analysis uses different classification approaches to devise the most accurate method applied. Methodologies and approaches applied in this project are:

1.Data wrangling: Non-meaningful slangs were replaced with their full forms. Data with duplicated indices were dropped to avoid any complications.

2. Data preprocessing: Data in textual format was converted into vectorised bag-of-words approach to convert each sentiment review into its equivalent feature matrix for classifier. Lemmatization and stemming was carried out to simplify similar terms. Term frequency-inverse document frequency was  used to emphasize more on words within the given minimum and maximum document frequency.

2.EDA (Exploratory data analysis): Infographics were created using pandas_profiler which provides a quick summary of data and shows the features with high correlation, value counts, distinct values, frequency distributions and so on.

3.Prediction model: Classification models such as decision trees, random forests, xgboost, naive bayes and support vector classifier were first evaluated to fit on the data set. However, due to the best performance of support vector classifier, it was chosen as the best fit and optimized for the labelled data. 

4.Cross validation: Cross validation is done on the final chosen model values.

An overall precision Metric for the test data came out to be 82.3%.

Conclusion: It can be seen that both XGBoost and Support Vector Classifier of linear kind prove equally useful in classifying the sentiments as positive, negative and neutral. Support vector classifier with hyperparameter tuning helps us achieve a precision of 83.2%.
