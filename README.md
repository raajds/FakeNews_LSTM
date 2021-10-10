# FakeNews_LSTM
About dataset :
The dataset consists of 3 CSV files: "train.csv", "test.csv" and "submit.csv".
"train.csv" contains following columns

"id" of article
"Title" of the article
"Text" of the article
"Author" of the article
"Label" of article
1: fake
0: real
"test.csv" contains the same attributes as "train.csv", but without the "label" 
attribute. Prediction is to be performed on these articles.

"submit.csv" contains sample submission format. For every article in "test.csv" 
file, submission CSV file should have two columns: `id` and `label`. The `id` 
column should refer to a row in the "test.csv" file, and the `label` column 
should refer to its label i.e. real (`0`), or fake (`1`).

# Output :
# Scope : This complete  Project is about fake news classifications through NLP 
  Language : Using Python and supporting packages and api, we will try to build this classification model 
  NLp : this is text news para, so we need to use python supporitng NLP packages 
  As per analysis we have independent variables and one that label column in data is called target
  classification, thought implementation is, we have title, author & text feature, since understanding
  is to classify Fake news to we will try to merge ‘title’ and ‘text’ and create on merged column.  

# Result :

              precision    recall  f1-score   support

           0       0.94      0.94      0.94      2087
           1       0.94      0.94      0.94      2073

    accuracy                           0.94      4160
   macro avg       0.94      0.94      0.94      4160
weighted avg       0.94      0.94      0.94      4160

# Confusion matrix

[[1966  121]
 [ 134 1939]]
 
#Saved output result with columns 'Id' and predicted label 'pred_lbl' with file name "LSTM_pred_submit.csv"
