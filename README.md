# COVID_19_Forecasting


## Data Exploration
  1. Extracting data from beginning to 17/May as the whole data set.
  2. Plotting bar chart for reviewing the porpotions of different Target types(If the Porpotion is skewed, the train test split part we should add some weight to avoid the skew data's impact).
  3. By sorting the TargetValue feature I found some negative value which is meaningless. I treated it as the wrong input and take the absolute value of these values.
  
## Data Cleaning
  1. Removal of missing value.
  2. take the absolute value of those wrong input values.
  3. Encoding 'Target', 'County', 'Province_State' features.

## Train Test Split
  1. The data prior to 10/May as the train data and the data after 10/May as the test data.
  
## Modeling
### Attempted Algorithms: 
  * Linear Regression: (R2 score:0.29)
  * Descion Tree Regression (R2 score:0.70)
  * Random Forest Regression (R2 score:0.37)
  * Extra Tree Regression (R2 score:0.90)
  * Gradient Boosting (R2 score:0.70)
  
## Evaluation
  1. adding columns that the loss function formula is needed
  2. Calculate the quantile part and weighted population part from the loss function formula, and finally multiply these two get the result
### the Weighted Pinball Loss score: 1.813281037325136


