# Machine Learning: Finding Optimal Model and Hyperparameters¶

### Project Overview 
The aim of this project is to develop an optimal predictive model for estimating car prices accurately. Leveraging machine learning techniques and advanced data analytics, the project seeks to create a robust model that accounts for various factors influencing car prices, such as make, model, year, mileage, and  features.


### Data Source
Vehicle dataset URL: (https://www.kaggle.com/datasets/nehalbirla/vehicle-dataset-from-cardekho)

### Tools
Python

### Data Understanding
In the initial data understanding step, we performed the following tasks:
- Data Loading and Inspection.
- Determined the total number of observations and fields.
- Analyzed the statistical characteristics of the numeric columns.
- Determined the data types of the columns.
- Calculated the total number of  null values.

 ### Data Preparation
 As part of preparing our dataset, we executed the following tasks:
 - Printed and dropped rows with null values.
 - Identified and removed duplicates rows.
 - Removed Outlier using the mean and standad deviation.

  ### Data Pre-Processing
  - Extracted only numeric values of the mileage, engine, and maximum power columns.

### Feature Engineering
- Dropped irrelevant features.
- Used one-hot encoding to change categorical data to numeric.
- Manually changed binary categorical data to numeric.

### Data Visualizations
We utilized data visualization to understand the relationship between each feature and the feature we want to predict.

### Model Building
- Splitted the dataset into train and test using the train_test_split module.
- The Grid search module was employed across various algorithms using different parameters to identify the optimal model.

### Results
- The Linear Regression accuracy was 64%.
- The Random Forest Regressor was 89%.
- When employing K-fold cross-validation on our Linear Regression, we achieved validation scores ranging from 57% to 64%.
- When employing K-fold cross-validation on our Random Forest, we achieved validation scores ranging from 87% to 91%.
- The grid search identified the decision tree as the best model, with the following parameters:  
  1.Criterion: Mean Square Error  
  2. Splitter: Best Split
