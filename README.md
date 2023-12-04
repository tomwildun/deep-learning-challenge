# deep-learning-challenge
Module 21 Challenge

**Analysis**

The target variable for the model is "IS_SUCCESSFUL". All remaining features are in the model with the exception of 'EIN' and 'NAME' as they were not needed for analysis. The Input layer was determined by the number of features in the data. I chose to use twice the number of features (n*2) for my first hidden layer. Second layer consisted of the same number of features as neurons (n*1).For each of the hidden layers ReLU activation function was used. The output layer was  neurons and used the Sigmoid activation function. Output for first run was as follows:

268/268 - 2s - loss: 0.5638 - accuracy: 0.7296 - 2s/epoch - 9ms/step
Loss: 0.5637978315353394, Accuracy: 0.7295626997947693

For optimized run, I used number of features * 3 for first hidden layer and number of features/2 for hidden layer 2.

268/268 - 2s - loss: 0.5598 - accuracy: 0.7290 - 2s/epoch - 6ms/step
Loss: 0.5597571134567261, Accuracy: 0.7289795875549316

I thought by increasing the number of neurons in hidden layer 1 and decresing the number of neurons in hidden layer 2 would increase the accuracy of the model

I then attempted to optimize the model by adding an additional hidden layer (3rd) with the same number of neurons as there are features within the df. 

268/268 - 2s - loss: 0.5656 - accuracy: 0.7278 - 2s/epoch - 7ms/step
Loss: 0.5656354427337646, Accuracy: 0.7278134226799011

My accuracy remained the same at 72% accuracy. I believe that experimenting with the number of neurons and hidden layers can get me to an accuracy above 75%. Other strategies that can improve accuracy: change activation functions, implement dropout regularization, adjust learning rate and optimizer, use batch normalization and increase training epochs or adjust batch size.



 
