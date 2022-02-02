# Neural Networks & Deep Learning Models

## Overview of the analysis
Using our knowledge of machine learning and neural networks, we will use the features in the provided dataset to help client create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

Client provided a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as the following:

- EIN and NAME—Identification columns
- APPLICATION_TYPE—Alphabet Soup application type
- AFFILIATION—Affiliated sector of industry
- CLASSIFICATION—Government organization classification
- USE_CASE—Use case for funding
- ORGANIZATION—Organization type
- STATUS—Active status
- INCOME_AMT—Income classification
- SPECIAL_CONSIDERATIONS—Special consideration for application
- ASK_AMT—Funding amount requested
- IS_SUCCESSFUL—Was the money used effectively

This assignment consists of three technical analysis deliverables and a written report. You will submit the following:

1. Deliverable 1: Preprocessing Data for a Neural Network Model
2. Deliverable 2: Compile, Train, and Evaluate the Model
3. Deliverable 3: Optimize the Model
4. Deliverable 4: A Written Report on the Neural Network Model (README.md)

## Results
Using bulleted lists and images to support your answers, address the following questions.

1. Data Preprocessing
- What variable(s) are considered the target(s) for your model?</p>
<i>"IS_SUCCESSFUL" are the targets. Determining/Predicting what is causing a project to be a success or failed.</i></p>
 
- What variable(s) are considered to be the features for your model?</p>
<i>APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT, and SPECIAL_CONSIDERATIONS are the features of the model.</i></p>
 

- What variable(s) are neither targets nor features, and should be removed from the input data?</p>
<i>EIN, and NAME are removed from the model and considered non-benficial.</i></p>


2. Compiling, Training, and Evaluating the Model
  - How many neurons, layers, and activation functions did you select for your neural network model, and why?</p>
   - <i>The model used 3 layers, with the first layer consisting of 80 neurons, layer two with 30, and the output layer with 1.</i></p>
   - <i>The activation functions for layer one and two used RELU, and the output layer used SIGMOID</i>
   - <i>ReLU was used to allow hidden layers to identify and train the nonlinear relationships in the dataset. Sigmoid is used for the output layer because the predictions are binary, either yes (Success) or no (Fail)</i>
  - Were you able to achieve the target model performance?</p>
  - <i>75% was the performance goal. The model accurancy was 69.49%</i></p>
  - What steps did you take to try and increase model performance?</p>
  - <i>Binning ASK_AMT into four bins, 5000 or less, 50000 or less, 1000000 or less, and over 1000000.</i></p>
   - This did not improve the model. It added more noise to the model which reduced accuracy.</p>
  - <i>other performace improvements included increasing the hidden layers from 2 to 3, and again from 3 to 4. Both additions did not improve the performace of the model.</i></p>
  
## Summary
Summarize the overall results of the deep learning model.</p>
<i>The model included a variety of features that lead to a noisy model. Removing some of the features or binning features could improve the model. Another potential improvement may be not using a deep learning model to process the data for predictions. An alternative is using a logistic regression because the targets for the model are binary.<i/>
