# BBC News Classification

In this, I first imported the required libraries and then imported the given dataset and converted them into dataframes. After that I encoded the different type labels into numeric format as any Machine Learning model can only operate on numbers.

After obtaining the data, I cleaned the data by
* removing punctuations
* stemming the words
* lemmatizing the words
* removing stop words
* converting text to lower case  

After this, I removed words whose frequency of occurence is lower than 3 as they won't contribute much in helping the model to understand their significance in the text

After this, I applied TF-IDF vectorization to the data to extract the import features i.e. words or trends present in the data. Then I created dictionaries to switch between encoded labels and original labels.

After this, I used the chi square analysis to find the most correlated words for each type. Then I plotted the data in 2D by using T-SNE to reduce the dimensions of data effectively.

After this, I checked four models 
* Logistic Regression Classifier
* Multinomial Naive Bayes
* Random Forest Classifier
* Support Vector Classifier

to find the model with best accuracy. They were as follows
| Model                  | Accuracy |
|------------------------|----------|
| LogisticRegression     | 0.975839 |
| MultinomialNB          | 0.973154 |
| RandomForestClassifier | 0.860403 |
| SVC                    | 0.928188 |

So, I chose Logistic Regression for the purpose of classification.
I split the Training set into training and validation sets in the ratio 2:1 and generated the confusion matrix for the prediction. The accuracy turned out to be 97.764 %.

Then I trained the Logistic Regressor on entire training data and applied it on the testing data to get the required output.



