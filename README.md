# Imbalanced Data with credit card fraud information 
This is a project were I going through how to solve an imbalanced classification problem. There are a lot more normal credit card transactions than their are fraudulent transactions. The issue is to decide which method and models to use to best solve how to predict what transaction is fraudulent or not. I picked undersampling and proceeded with logistic regression after testing how a few other models. This data was taken off of kaggle and can be found here: https://www.kaggle.com/dalpozz/creditcardfraud


## How I went about this project: 

1) Download the data off of kaggle at the site above

2) I looked through the data to see how imbalanced the classifications were
  - I viewed the length of the lists and also plotted it on a graph to get a visual representation
  
3) To continue with modeling I first wanted to standardize the amount column. Given it was at different different rations compared to the PCA data, I scaled it down so that the cost function could run faster 

4) I then created a seperate data frame for the undersampled data to then run analaysis

5) I modeled the data using SVM, Decision Trees, Random Forests and Logistic Regression. I viewed their accuracies as now the data is balanced to find the best model to use for the entire data set. 

6) I found that the Logistic Regression was actually the best model to use on the entire imbalanced data set.

Running the tests
The tests actually ran pretty quickly. The dataset its self isn't too large, so testing how different models and parameters is suggested. Given they already gave us the principal componenets I did not try to do feature engineering. I did get rid of the time variable as I didn't find it that useful.

Acknowledgments
Thanks to joparga3 off of Kaggle for inspiration and the code to find the best C parameter. 
