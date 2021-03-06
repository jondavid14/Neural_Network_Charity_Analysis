# Neural_Network_Charity_Analysis

## Overview

Using my knowledge from machine learning and neural networks for this project I use the features in this dataset I create a binary classifier that will tell the customer whether or not the applicants will be successful using alphabet soup.

## Results
- **Data Processing**
   - Removed the EIN and NAME columns because they did not contribute to the model
   - The varibales  for my model are:
    'STATUS', 'ASK_AMT', 'IS_SUCCESSFUL', 'APPLICATION_TYPE', 'CLASSIFICATION', 'USE_CASE', 'ORGANIZATION', 'INCOME_AMT'. I dropped "USE_CASE_Other","AFFILIATION_Other" columns. 
    - the dependant variable "IS_SUCCESFUL"  
   
- **Compiling, Training, and Evaluating the Model**
  **Attempt #1**
   - 2 Hidden Layers
   - 80 neurons (Layer1), 30 neurons(Layer2)
   - Used Relu and Sigmoid Activations Functions since sigmoid is best for binary classifcation problems as this and relu is for nonlinear datasets.
   - Removed "USE_CASE_Other","AFFILIATION_Other" columns. 
   
<img width="485" alt="Screen Shot 2020-11-22 at 6 11 13 PM" src="https://user-images.githubusercontent.com/67808057/99924221-30f2f700-2cee-11eb-96f0-2522d49b3dc9.png">

   
   
  **Attempt #2**
   - 3 Hidden Layers 
   - 80 neurons (Layer1), 30 neurons(Layer2), 15 neurons(Layer3)
   - Used Relu and Sigmoid Activations Functions since sigmoid is best for binary classifcation problems as this and relu is for    nonlinear datasets.
   - Removed "USE_CASE_Other","AFFILIATION_Other" columns. 
   
   <img width="466" alt="Screen Shot 2020-11-22 at 5 37 49 PM" src="https://user-images.githubusercontent.com/67808057/99924049-8c70b500-2ced-11eb-88f9-763a8606a644.png">
   
   
  **Attempt #3**
   - 3 Hidden Layers
   - 80 neurons(Layer1), 35 neurons(Layer2), 10 neurons (Layer3)
   - Used Relu and Sigmoid Activations Functions since sigmoid is best for binary classifcation problems as this and relu is for    nonlinear datasets.
   - Went back to original dataset 
   
   <img width="507" alt="Screen Shot 2020-11-22 at 6 08 54 PM" src="https://user-images.githubusercontent.com/67808057/99924141-df4a6c80-2ced-11eb-8648-58d4fbed4155.png">
   
 **Attempt #4**
  - 3 Hidden Layers
  - 80 neurons (Layer1), 30 neurons(Layer2), 15 neurons (Layer3)
  - Reordered Relu and Sigmoid Activations 
  - Went back to original dataset
  
  
I tried to change my models in order to achieve a more than 75% accuracy rate but only got about 73%. I changed my features, activation functions, Hidden Layers, and the number of neurons in order to achieve this. But if one where to get this result it would take longer than a more than expected so I am content with the results I got in one day. 
  
## Summary 
On Average my models kept around 73% accuracy score which is decent considering it was an improvement. My recommendation to improve this model would be to find better features to help explain what determines "IS_SUCCESFUL" such as more indepth knowledge of the other associates/ firms being funded. At the end of the day, knowledge is power and if we had more indepth data between all these applications, we can create a better model.
