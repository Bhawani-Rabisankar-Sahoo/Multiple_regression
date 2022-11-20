# Multiple_regression
Multiple regression using XGboost 





## Approach
 

First I've just used the basic multiple regression model and got around **70%** efficiency .

After that I used Xgboost in my model which significantly increased the efficiency to **81%**.

Then I went for Hyperparameters in Xgboost and tested RandomSearchCV and 

GradientSearchCV in which GradientSearchCV has **90.833%** efficiency  and RandomSearchCV

has **91%** efficiency so I went for RandomizedSearchCV.

In all above models I've splited the training set into two parts by using train_test_split

where training set has 70% data and testing set has 30% data.
## Implementation      


This repository has two folders 'solution'  and 'code'

'code' folder has 5 files 

- train.py
- test.py
- trainingdata.csv
- testingdata.csv
- Multiple_Regression_Topcoder.pkl

In train.py 

please paste training data path between Single Quotation Marks (‘ ’) like  '.....Paste Here.....' 

```
df = pd.read_csv('/content/trainingdata.csv' , names = range(46))      #loading trainingdata          
                 #'....Training data path.....'

```
In test.py

paste testing data path
```
df_test = pd.read_csv('/content/testingdata.csv' , names = range(45))  #testing data
                 #'....Testing data path........' 
```

if it doesn't work by default then paste the  Multiple_Regression_Topcoder.pkl path between Single Quotation Marks (‘ ’) like'.....Paste Here.....'
```
clf_from_joblib = joblib.load('Multiple_Regression_Topcoder.pkl')  
                               #'.............path.............' 

```

I've done the training and testing in   Google Colab

train.py notebook link  "https://colab.research.google.com/drive/1bVam9IVEPoJAlae-6oT400qQ0RNm2Va_?usp=sharing"

test.py notebook link   "https://colab.research.google.com/drive/1wrm6QkBrun0kYzkd30K14oaCPn3VARmr?usp=sharing"

It will be easier for you if you just click the  links and use the notebooks

Then  upload the trainingdata.csv  ,   testingdata.csv   ,  Multiple_Regression_Topcoder.pkl in the root folder and everything will be fine.

