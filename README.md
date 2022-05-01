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
- I wasn't able to achieve the 75% target. I had tried different number of layers, neurons and activations, but not able to get to the target.
- Steps to increase the model performance
  - I have eliminated the featured 'ASK_AMT'

    <img src='https://github.com/juliomeza/Neural_Network_Charity_Analysis/blob/main/screenshot/ask_amt_plot.png'>
    
  - I have increased the number of layers and neurons
  - I have used a combination of different activations (relu and tanh)
  - I have run the optimizer several times to find the optimal model.

## Summary
- The model can predict whether applicants will be successful if funded by Alphabet Soup with an accuracy of 72%.
- Because of the small amount of data, a Random Forest may have a better prediction rate.
- Eliminating more feautures may help improve the model.