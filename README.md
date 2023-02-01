# Web-Scrapping-and-Machine-Learning

## Problem 1

Write a web scraping script which takes an input of any film actor and gives the output of filmography of that actor in descending order.


<hr><hr>

## Problem 2

Given a list of planets discovered by KEPLER.

Kepler Data: https://drive.google.com/drive/folders/1GwqC4STc_KgVPofacQUzKHBMHQsmflvY?usp=sharing

Create an ML algorithm to classify the planets as Candidate/False positive/Confirmed etc based on the  column “koi_disposition”.
y

## Sub-questions for Problem 2

Why did you choose the particular algorithm?<hr>
Combinations of several algorithms via ensemble techniques although on selecting one from all, the randomForest classifier works best

<hr><hr>

What are the different tuning methods used for the algorithm?<hr>
Hyperparameter tuning, and standardization methods were used<hr>
("rf_model", RandomForestClassifier(bootstrap=False, max_depth=80, min_samples_leaf=2,
                       min_samples_split=5, n_estimators=600, random_state=24)),
        ("xgb_model", XGBClassifier(eval_metric="logloss", random_state = 18)),
        ("svm_model", SVC(C=1000, gamma=0.01))<hr><hr>
        
        
        
Did you consider any other choice of algorithm?Why or why not?<hr>
Considered 4 individual algorithms and then the combinations of them which were finally selected via voting classifier

<hr><hr>
What is the accuracy?
On Train Data<hr>
Accuracy: 0.8570541673133634<hr>
F1 Score: 0.8570541673133634<hr>
Precision: 0.8570541673133634<hr>
Recall: 0.8570541673133634<hr>

On Test Data<hr>
Accuracy: 0.8590937306021105<hr>
F1 Score: 0.8590937306021105<hr>
Precision: 0.8590937306021105<hr>
Recall: 0.8590937306021105<hr>
<hr>

What are the different types of metrics that can be used to evaluate the model?<hr>
Accuracy, F1 Score, Precision, Recall, Confusion Matrix

