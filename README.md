# deep-learning-challenge

## Purpose of the analysis
The purpose of this anaylysis was to create a model that would be able to predict which applicants to a nonprofit for funding would be the most likely to successful at their projects.

## Data Processing
### Target variable
The target variable is whether or not a project is successful, coded as 0 and 1
### Model features
The features for the model are,
  *application type
  *affiliation, classification, use_case, organization, status, income_amt, and ask_amt
### Variables removed because they are neither targets or features
EIN and Name were removed from the data set because they were neither targets or features
### Compiling, Training, and Evaluating the Model
TensorFlow was used to define the model, then it was compiled so it could be trained, the model was then trained using 100 epochs, with one of the attempts to optimize the model using 250 epochs.
## Neurons, layers, and activation functions selected for model and why?
For the original model in the AlphabetSoupCharity file two hidden layers were used, the first hidden layer had 27 neurons and the second one 25. I used these numbers becuase there was a relatively high numbers of features in the model. The activation functions used were, sigmoid for the base layer becuase the dataset has a binary classification, and relu for the hidden layers becuase the data was both positive and nonlinear.
## Were you able to achieve the target model performance?
I was not able to achieve the target performance of the model. The highest accuracy I was able to achieve was 72.77%.

## What steps did you take in your attempts to increase model performance?
The orginal model had an accuracy of 72.42%. In the first attempt to improve the model I added an additional hidden layer, this improved the accuracy of the model slightly to 72.71%. In the next attempt at the model I increased the number of nodes in one of the hidden layers, this again slightly improved the performance of the model, but only to 72.77%. The final attempt saw an accuracy of 72.75%, in this model there was both the extra layer and the increased number of neurons, I also changed the activation function in the hidden layers from relu to leaky relu, and ran 250 epochs instead of 100 as for the previous models. While all of the attempts at optimization saw an improvement over the original model nome of them reached 75% accuracy.
All of the models are in the models folder.

## Summary
While the results are fairly predicitive of if a funded project will be successful or not there is still a fair amount of room left for improvement in the model. One way to improve the model could be using a random forest algorithm. Taking smaller samples of the data for each tree could help with the issue that several of the features have a large proportion of projects in one category but then also a specific proportion of projects that fall within other categories.

