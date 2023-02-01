# Web-Scrapping-and-Machine-Learning

Problem 1

Write a web scraping script which takes an input of any film actor and gives the output of filmography of that actor in descending order.

Use web scraping method

Eg : 
input [Leonardo DiCaprio]
Output : Films done by Leonardo DiCaprio in descending order

Time Limit:1 Day

Problem 2

Given a list of planets discovered by KEPLER.

Kepler Data: https://drive.google.com/drive/folders/1GwqC4STc_KgVPofacQUzKHBMHQsmflvY?usp=sharing

Create an ML algorithm to classify the planets as Candidate/False positive/Confirmed etc based on the  column “koi_disposition”.


Time Limit:1 Day

Sub-questions for Problem 2

Why did you choose the particular algorithm?
Combinations of several algorithms via ensemble techniques although on selecting one from all, the randomForest classifier works best



What are the different tuning methods used for the algorithm?
Hyperparameter tuning, and standardization methods were used
("rf_model", RandomForestClassifier(bootstrap=False, max_depth=80, min_samples_leaf=2,
                       min_samples_split=5, n_estimators=600, random_state=24)),
        ("xgb_model", XGBClassifier(eval_metric="logloss", random_state = 18)),
        ("svm_model", SVC(C=1000, gamma=0.01))
        
        
        
Did you consider any other choice of algorithm?Why or why not?
Considered 4 individual algorithms and then the combinations of them which were finally selected via voting classifier


What is the accuracy?
On Train Data
Accuracy: 0.8570541673133634
F1 Score: 0.8570541673133634
Precision: 0.8570541673133634
Recall: 0.8570541673133634

On Test Data
Accuracy: 0.8590937306021105
F1 Score: 0.8590937306021105
Precision: 0.8590937306021105
Recall: 0.8590937306021105


What are the different types of metrics that can be used to evaluate the model?
Accuracy, F1 Score, Precision, Recall, Confusion Matrix

