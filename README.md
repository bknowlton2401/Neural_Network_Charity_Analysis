# Neural_Network_Charity_Analysis
To use machine learning and neural networks and use the features in the provided dataset to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

## Overview of the analysis
The purpose of this analysis was to predict if applicants would be successful if funded by Alphabet Soup Co. To help Alphabet Soup Co. determine which companies and give a prediction accuracy percentage, we processed the data, compiled, trained and evaluated the module by deleting unnecessary columns and hidding layers. 

## Results
 - Data Preprocessing
  - The data was cleaned by removing EIN and NAME columns since their information does not affect the accuracy prediction.
  - The variables/columns considered for the model are: 'STATUS', 'ASK_AMT', 'IS_SUCCESSFUL', 'APPLICATION_TYPE', 'CLASSIFICATION', 'USE_CASE', 'ORGANIZATION', 'INCOME_AMT'. 
  - We also dropped "USE_CASE_Other","AFFILIATION_Other" columns because these also do not affect the prediction accuracy. 
  - We kept the dependent variable as "IS_SUCCESSFUL" since this does effect the prediction accuracy. 
 
 - Compiling, Training, and Evaluating the Model
  - Attempt #1
   - Used 2 hidden layers (80 neurons (layer1) and 30 neurons (layer2)
   - Removed "USE_CASE_Other","AFFILIATION_Other" columns.
   - Accuracy = 72%
  
  ![accuracey 72](https://user-images.githubusercontent.com/96890065/175837149-f25926ae-bed3-4f0b-ae61-4f1ac62fee14.JPG)
  
  - Attempt #2
   - Created 2 more hidden layers
   - This did not improve the accuracy
   - Accuracy = 71.8%
   
   ![accuracy 71](https://user-images.githubusercontent.com/96890065/175837199-2a567e96-fddb-4550-acb3-d7d998d8c399.JPG)

  - Attempt #3
   - Refined hidden layers
   - Still no improvement
   - Accuracy = 72%
   
   ![acc 72](https://user-images.githubusercontent.com/96890065/175837242-85e4a55b-84a9-47fb-b027-1ce88e44bed8.JPG)
   
   ## Summary
   Overall I was not able to get my prediction accuracy above 72%.  I would need get a better understanding of each column to see if more could be dropped or change the hidden layers. 
