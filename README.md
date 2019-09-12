# DUPLICATE-QUESTION-PREDICTION-IN-QUORA-DATASET

### It is a binary classification problem, for a given pair of questions we need to predict if they are duplicate or not. </p>

#### OBSERVATIONS:

![Screenshot (81)](https://user-images.githubusercontent.com/48092244/64814574-50a66f80-d5c1-11e9-8128-c7389bfc7ab9.png)

### Procedure :
1] Firstly we are combining all the features which we have engineered earlier.<br>
2] Before building a model we are combining both the question1 and question2 in to one dataframe and then adding all the features in to this dataframe.<br>
3] After building dataframe we are splitting into train and test (70-30).<br>
4] Then we are applying tfidfvectorizer on the text data which are combination of question1 and question2.<br>
5] Further we are hstacking both the tfidfvectorizered features with the features which we have engineered.<br>
6] We then build a Logistic regression, Linear SVM and XGBOOST model. XGBOOST implementation gave test logloss of 0.316.<br>
7] Then we are applying tfidf weighted W2V on the text data which are combination of question1 and question2 and by building an XGBOOST model on this text we get test Logloss of 0.3157.
