# Neural Network Charity Analysis

## Overview
Create a deep learning classification model to predict whether applicants will be successful if funded by Alphabet Soup.

## Results
### Data Preprocessing
- The target variable is the 'IS_SUCCESSFUL' column.
- Feature variables
  | Features  | Unique Values |
  | ------------- | ------------- |
  | APPLICATION_TYPE  | 17  |
  | AFFILIATION  | 6  |
  | CLASSIFICATION  | 71  |
  | USE_CASE  | 5  |
  | ORGANIZATION  | 4  |
  | STATUS  | 2  |
  | INCOME_AMT  | 9  |
  | SPECIAL_CONSIDERATIONS  | 2  |
  | ASK_AMT  | 8747  |
- The 'EIN'and 'NAME' are neither target nor features and should be removed from the input data.

### Compiling, Training and Evaluating the Model
- I have used 3 layers with 84, 69 and 41 neurons on each layer beacuse that is what the Optimizer returned. For the activations, I used a combination of relu and tanh as recomended by the optimizer as well.
  <img src='https://github.com/juliomeza/Neural_Network_Charity_Analysis/blob/main/screenshot/BestModel.png'>
  <img src='https://github.com/juliomeza/Neural_Network_Charity_Analysis/blob/main/screenshot/Model.png'>

## Summary