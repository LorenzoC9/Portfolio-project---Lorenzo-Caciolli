# Datasheet Template

As far as you can, complete the model datasheet. If you have got the data from the internet, you may not have all the information you need, but make sure you include all the information you do have. 

The reference database was found from the following source: https://archive.ics.uci.edu/ml/datasets/HCV+data

## Motivation

- For what purpose was the dataset created? 
The dataset was built in order to study the correlation of several blood biomarkers (e.g., proteins and enzyme) characteristics for liver function, to the stage of liver disease in patients affected by hepatitis C. 

- Who created the dataset (e.g., which team, research group) and on behalf of which entity (e.g., company, institution, organization)? Who funded the creation of the dataset?
The database was created and donated by Ralph Lichtinghagen, Frank Klawonn, Georg Hoffmann. The creator worked on behalf of several corresponding institution: 
- Ralf Lichtinghagen: Institute of Clinical Chemistry; Medical University Hannover (MHH), lichtinghagen.ralf '@' mh-hannover.de;
- Frank Klawonn; Helmholtz Centre for Infection Research; Braunschweig, Germany, frank.klawonn '@' helmholtz-hzi.de;
- Georg Hoffmann; Trillium GmbH; Grafrath, Germany; georg.hoffmann '@' trillium.de

No information about the funding for the establishment of the database
 
## Composition

- What do the instances that comprise the dataset represent (e.g., documents, photos, people, countries)? 
The dataset contains laboratory values of blood donors and Hepatitis C patients and demographic values like age. Laboratory values involve the expession found in blood sample of the following proteins or enzymes: albumin (ALB), alkaline phosphatase (ALP), alanine amino-transferare (ALT), aspartate amino-transferase (AST), bilirubin (BIL), choline esterase (CHE), cholesterol (CHOL), creatinine (CREA), gamma-glutamyl transferate (GGT), total protein (PROT). Patients' sex is also involved in the predictors. 

- How many instances of each type are there? 
The full dataset contains 615 instances with 14 overall attributes. 

- Is there any missing data?
Yes, the dataset involves missing data. The total number of missing valyes is 31.

- Does the dataset contain data that might be considered confidential (e.g., data that is protected by legal privilege or by    doctor–patient confidentiality, data that includes the content of individuals’ non-public communications)?
Yes, the dataset may contain data that might be considered confidential. This involve demographic and gender information, as well as results coming patients from blood analysis. 

## Collection process

- How was the data acquired? 
Data was collected as the direct processing of blood test looking for key metabolic hepatic functions. 

- If the data is a sample of a larger subset, what was the sampling strategy? 
The source does not mention any potential larger sets and eventual sampling strategies

- Over what time frame was the data collected?
No information regarding the timeframe over which data was collected. The database was donated on 2020-06-10. 

## Preprocessing/cleaning/labelling

- Was any preprocessing/cleaning/labeling of the data done (e.g., discretization or bucketing, tokenization, part-of-speech tagging, SIFT feature extraction, removal of instances, processing of missing values)? If so, please provide a description. If not, you may skip the remaining questions in this section. 
The source does not mention any preprocessing/cleaning/labelling of the data. However, data was further preprocessed in the algorithm in the following steps: 
- elimination of datapoints containing missing values 
- conversion of categorical predictors (e.g., sex = male, female) in numerical outcome (e.g., sex = 0, 1)

- Was the “raw” data saved in addition to the preprocessed/cleaned/labeled data (e.g., to support unanticipated future uses)? 
Yes, the full dataset was probably storage in its raw data version to be further undergoing prepocessing from the users. 
 
## Uses

- What other tasks could the dataset be used for? 
The dataset has been described to be used only for the purpose of predicting the stage of hepatic disease in hepatitis C patients. No toher uses are described from the source. 

- Is there anything about the composition of the dataset or the way it was collected and preprocessed/cleaned/labeled that might impact future uses? For example, is there anything that a dataset consumer might need to know to avoid uses that could result in unfair treatment of individuals or groups (e.g., stereotyping, quality of service issues) or other risks or harms (e.g., legal risks, financial harms)? If so, please provide a description. Is there anything a dataset consumer could do to mitigate these risks or harms? 
The dataset is published in its raw form, without any explicit preprocessing/cleaning/labelling bein performed. This fact allowed the database to be used by several users who might want to preprocess/clean/label it according to their necessities. 

- Are there tasks for which the dataset should not be used? If so, please provide a description.
The source does not mention any tasks for which the databse should not be used. 

## Distribution

- How has the dataset already been distributed? 
The dataset has been donated to the UCI machine learning repository on 2020-06-10. Since then, it has been available online for consultation and download.

- Is it subject to any copyright or other intellectual property (IP) license, and/or under applicable terms of use (ToU)?
No information was reported regarding potential copyright or intellectual property license. 

## Maintenance

- Who maintains the dataset?
The dataset is currently online and publicly available on the UCI machine learning repository webpage (https://archive.ics.uci.edu/ml/datasets/HCV+data)
