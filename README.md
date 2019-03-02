# work_sample

### Using machine learning for predictive maintenance
Build a model for customer, 3D Technologies, that determines the optimal time for when maintenance should be performed (optimal time = minimize false positives and false negatives). 

### Outline
target = ['failure']
features = ['attribute1', 'attribute2', 'attribute3', 'attribute4', 'attribute5', 'attribute6', 'attribute7', 'attribute8', 'attribute9','Dayofweek']

1. Clean and transform data
2. Exploratory Data Analysis (EDA)
 * Check if we're dealing with imbalanced classes
3. Modeling & evaluation (classification models)
 * Train-test-split
 * 
4. Conclusion
 * What are the performance targets that the model should be optimized for? High precision, high sensitivity/recall, high accuracy? What is the consequence of not predicting a failure or predicting a failure that will not happen?
5. Clean code with classes & functions

### Given time constraints and the nature of this exercise, I decided to take a "quick and dirty" approach. Some things I skipped over were:
* Train-test-split the data before scaling
* Feature selection (SelectKBest, SelectFromModel, SelectPercentile, RFE, etc.)
* Use pipelines to chain tasks from preprocessing to modeling, to evaluate multiple models in a convenient way.
