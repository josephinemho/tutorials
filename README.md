# work_sample

### Using machine learning for predictive maintenance
Build a model for our customer, 3D Technologies, that determines the optimal time for when maintenance should be performed (optimal time = minimize false positives and false negatives). 

### Outline
target = ['failure']
features = ['attribute1', 'attribute2', 'attribute3', 'attribute4', 'attribute5', 'attribute6', 'attribute7', 'attribute8', 'attribute9','Dayofweek']

1. Clean and transform data
2. Exploratory Data Analysis (EDA)
3. Handle imbalanced classes
4. Modeling & evaluation
5. Conclusion


### Given time constraints and the nature of this exercise, I decided to take a "quick and dirty" approach. Some things I skipped over were:
* Train-test-split the data before scaling
* Feature selection (SelectKBest, SelectFromModel, SelectPercentile, RFE, etc.)
* Use pipelines to chain tasks from preprocessing to modeling, to evaluate multiple models in a convenient way. 
* Try under-sampling instead of over-sampling. After trying our models on both resampled and non-resampled data, the models didn't do that much better on either one consistently. Given the nature of our data (we have a ton of failure=0 events), it could have been better to undersample and reduce the abundant class. Oversampling might actually be more appropriate when there isn't sufficient data (whereas in our case, we have sufficient data, it's just imbalanced). 
* Put everything into classes/functions and clean code