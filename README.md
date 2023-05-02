# Project portfolio - predicting liver disease in Hepatitis C patients


## NON-TECHNICAL EXPLANATION OF YOUR PROJECT
The identification of a disease stage could be very complex, sometimes involving the necessity of invasive measurements. In this context, the use of key metabolic markers has been recently described as a valuable tool for non invasive, but very efficient disease diagnostics.
The present application concerns the development of a machine learning tool for the classification of end-stage liver disease in patients affected by Hepatitis C.
The reference database concerns a cohort of both female and male individuals. The dataset contains several metabolic predictors (e.g., serum albumin level, gamma glutamyl transferase etc.) and one categorical outcome corresponding to the stage of the disease (e.g., hepatitis, fibrosis, cirrhosis,etc.). Based on the predictors, the main aim of the model is to correctly classify the stage of liver disease progression in the patients’ cohort.


## DATA
Each data instance relates to different patients involved in the study. Each data instance is evidenced with a different patient number. The dataset contains 615 data instances with 12 total predictors and 1 outcome variable representing the stage of the pathology. 
The predictors in the dataset are mainly numerical (e.g., float64). The only categorical predictor concerns the sex of the individual involved in the study. Therefore predictor “Sex” may relate to a male or female individual. 
Other predictors relate to the metabolic expression of key proteins and enzymes characterizing liver functions. These involve albumin (ALB), alkaline phosphatase (ALP), alanine amino-transferare (ALT), aspartate amino-transferase (AST), bilirubin (BIL), choline esterase (CHE), cholesterol (CHOL), creatinine (CREA), gamma-glutamyl transferate (GGT), total protein (PROT). These values are generally obtained by simple blood test analysis and are represented by numerical data. 
The dataset involves an outcome categorical variable concerning the stage of the hepatic disease. This involved the following categories: blood donor (meaning healthy individual), suspected blood donor (suspected healthy individual), hepatitis, fibrosis and cirrhosis. 
The source of the database is the following: https://archive.ics.uci.edu/ml/datasets/HCV+data


## MODEL 
The present machine learning model develops decision trees for classification purposes. The choice of this particular model structure was driven by several aspects. Decision trees are generally easy to be interpreted and explained. Explainability is always an important feature whenever dealing with healthcare and clinical-related aspects. Moreover, decision trees do not suffer a heavy and time consuming hyperparameter optimization as found in other models in machine learning (e.g., fully connected neural networks). 
The model performance was assessed in the overall model accuracy on the test set obtained as a portion of the full dataset.  


## HYPERPARAMETER OPTIMSATION
The hyperparameters concerned in this application involved: 
-	tree depth (max_depth), 
-	the number of features to consider when looking for the best split (max_features), 
-	The minimum number of samples required to be at a leaf node (min_sample_leaf)
-	The minimum number of samples required to split an internal node (min_sample_split)
Hyperparameter optimization was carried out by traditional grid search methods analysing the whole possible combinations of hyperparameters. This was decided as the most suitable method given the contained amount of hyperparameters to be optimized.


## RESULTS
The full dataset was split into a training a test subset. Decision trees hyperparameters were optimized and the model was further trained on the training set. The result concerned model classification accuracy on the test set demonstrated to be higher than 96%.  

## (OPTIONAL: CONTACT DETAILS)
If you are planning on making your github repo public you may wish to include some contact information such as a link to your twitter or an email address. 

Twitter account: lorenzocaciolli (@lorenzocaciolli)
