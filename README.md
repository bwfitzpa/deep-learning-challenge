# deep-learning-challenge

## Purpose of the analysis
The purpose of this anaylysis was to create a model that would be able to predict which applicants to a nonprofit for funding would be the most likely to successful at their projects.

## Data Processing
### Target variable
The target variable is whether or not a project is successful, coded as 0 and 1
### Model features
The features for the model are application type, affiliation, classification, use_case, organization, status, income_amt, and ask_amt
### Variables removed because they are neither targets or features
EIN and Name were removed from the data set because they were neither targets or features
### Compiling, Training, and Evaluating the Model
TensorFlow was used to define the model, then it was compiled so it could be trained, the model was then trained using 100 epochs, with one of the attempts to optimize the model using 250 epochs.
## Neurons, layers, and activation functions selected for model and why?
For the original model in the AlphabetSoupCharity file two hidden layers were used, the first hidden layer had 27 neurons and the second one 25. I used these numbers becuase there was a relatively high numbers of features in the model. The activation functions used were, sigmoid for the base layer becuase the dataset has a binary classification, and relu for the hidden layers becuase the data was both positive and nonlinear.
## Were you able to achieve the target model performance?
I was not able to achieve the target performance of the model. The highest accuracy I was able to achieve was 0.

## What steps did you take in your attempts to increase model performance?

## Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.



Write an analysis that includes a title and multiple sections, labeled with headers and subheaders (4 points)
Format images in the report so that they display correction (2)
Explain the purpose of the analysis (4)
Answer all 6 questions in the results section (10)
Summarize the overall results of your model (4)
Describe how you could use a different model to solve the same problem, and explain why you would use that model (6)

For this part of the assignment, you’ll write a report on the performance of the deep learning model you created for Alphabet Soup.


Results: Using bulleted lists and images to support your answers, address the following questions:

