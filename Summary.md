# deep-learning-challenge

## Overview 
The purpose of this analysis is to evaluate the performance of a deep learning model developed for Alphabet Soup, a hypothetical charity funding organization. The model aims to predict the success of charity applications based on various features extracted from the application data.



## Results

### Data Preprocessing
- The targets for the module is the 'IS_SUCCESSFUL' variable of the dataset.
- The variables for the features of the model consists of all columns from the original dataset except 'IS_SUCCESSFUL', 'EIN', and 'NAME'.
- The two non-beneficial columns initially are 'EIN' and 'NAME'. Later during optimizations, the 'AFFILIATION', 'USE_CASE', and 'ORGINATION' columns were dropped in an attempt to improve model accuracy.

### Compiling, Training, and Evaluating the Model

- In the initial model, there were two hidden layers using the Relu functions. The first layer had 80 neurons, and the second layer had 30 neurons. In optimizations, an additional layer was added using Relu and 125 neurons to improve accuracy. All models had a final output layer using Sigmoid and 1 neuron. The number of neurons/layers was chosen as 2 - 3 layers is typically enough layers to complete most models. 
- With the current model and optimization parameters, I was only able to achieve a 72% accuracy. This is below the target of 75%. 
- Steps to improve performance included adding more neurons in each layer, adding a third hidden layer, dropping more columns from the original dataset, and adjusting the testing split ratio of data. 


## Summary
Overall, the total accuracy of the model is around 72%. When attemping to optimize the model to achieve at least 75%, the following optimizations were made:
- Increasing the number of neurons in each layer
- Decreasing the number of neurons in each layer
- Adding an additional layer using Relu
- Dropping more columns from the original dataset
- Adjusting the testing split ratio of data

Unfortunately, I did not achieve getting the accuracy to at least 75% across three different optimization attempts.

## Resources Used
- https://www.tensorflow.org/api_docs
- https://scikit-learn.org/stable/
- https://www.tensorflow.org/model_optimization