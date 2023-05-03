# Model Card

See the [example Google model cards](https://modelcards.withgoogle.com/model-reports) for inspiration. 

## Model Description

**Input:** Numerical data (demographical and biochemical data)

**Output:** Classification of a data instance in a different category according to the value of the inputs. The categories involve healthy conditions (Blood donor), suspected healthy conditions (Suspected blood donor) and hepatic pathological conditions (hepatitis, fibrosis, cirrhosis). 

**Model Architecture:** Decision tree for classification purpose with hyperparameter optimization carried out with grid search method. 

## Performance

The performance was quantifies in the overal classification accuracy over the entire dataset. The model was trained on a training set and its performance was further evaluated on new - unseen - data (test set). 

## Limitations

Data instance disparities:
The overall model performance may be impacted by the disparity of data instances from each of the concerned categories in the training set. When focusing on a specific category (e.g., correctly classifying fibrosis instances), it would be necessary to carry out oversampling techniques to re-establish proportionalities within the dataset. 

Different scale of predictors:
Model performance may be affected by the different scales (and potentially different experimental setups) used to obtain the biochemical predictors.

Presence of several missing values: 
The model's performance may suffer the presence of multiple missing values in the dataset. Often, biomarkers expressions are generally independent from each other. Therefore, the most common strategy to deal with missing data is generally represented by removing those instances. 

## Trade-offs

The model displays higher performance on the test set (overall accuracy) whenever model hyperparameters were previously optimized before. 
When focusing on a specific target (e.g., category = fibrosis), oversampling techniques (via stratified sampling algorithm) allowed a higher accuracy in the detection of the instances from the class of interest. 
