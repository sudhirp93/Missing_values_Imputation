# Missing_values_Imputation

Data Collection: Took the BeerRecipeData from Kaggle in csv format

Data Cleaning: Two columns with more than 90% missing values were dropped as these two will be of no use in making models and 3 columns (with missing values) were taken into considerations todo missing value imputation.

1. Mean/Mode/Median Imputation: Replaced the missing values with mean in the dataset and there were no change in the before and after mean value of the columns as this could be a valid approach here.

2. Simple Imputer(Mean imputation): Here I used simple imputer module from scikit library and handled the missing values with mean of the respective columns.

3. Deductive Univariate Imputation (Simple Imputer): Used to replace 17.78 value with mean (just for practice)

4. Multivariate Regression Imputation (Iterative Imputer): Imported Iterative imputer form scikit library. Prepared the subset of numerical variables those have missing values. Fit the subset into the model with a fixed number of iteration and it transformed the missing values with the best fitted values.

5. KNN Imputation: Imported KNNImputer from scikit library and fit the subset into the model with fixed number of neighbors (high the number of neighbors lesser will be the chance of biasing) and then it transformed the missing values with the best fitted values.
