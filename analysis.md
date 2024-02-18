### Overview 
The purpose of this analysis is to gather the data in order to make predictions on the success of the Alphabet Soup Charity campaign to make more imformed decisions and improve the outcome of the charity overall. For example, building a machine learning model can predict the necessary factors that are needed to ensure success in raising money for the charity. 
### Results
* Data Preprocessing
    * The target variable for this model was "IS_SUCCESSFUL" which determined the success of the fundraising campaign with a specifc affiliation they were requesting money from.

    * The feature variables were everything else in the dataset (included in the picture). These became the factors that determined if the campaign was successful or not.
      
   * ![Columns](https://github.com/chris-levine/deep-learning-challenge/assets/143342297/96ee9b81-ea52-4296-877a-45d4c6daf72d)

    * The variables that were removed from the data set were "NAME" and "EIN" because they were solely unique identifiers and didn't give any informatiom whether the campaign would be successful or not. In other words, they do not contribute to the predictive power of the model

* Compiling, Training, and Evaluating the Model
    * I selected in total 160 neurons spanned across four different hidden layers. Furthermore, I used "relu" activation and "sigmoid" activation for the output layer. I used 160 neuron across four hidden layers due to the complexity of the model. If I used less than that the model wouldn't completely capture the complex patterns in the data. Furthermore, I used the "relu" activation function in the input and hidden layers because it sort of is the default standard. However, I used the sigmoid function in the output layer because predicted outputs are either (0 or 1) so it is only trying to binarily classify the outcomes. 
    * I was not able to achieve my target model performance.
    * Some things I tried to do was to add more neurons to each layer and also increase the amount of layers. Furthermore, I also binned another column ("ASK_AMT") because the majority of the asking amount was 5000. I took everything higher than 5000 and added it to a bin. 

* Summary
    * Overall the model performed not as well as I would have liked it to. Especially after re-preprocessing the data and adding more neurons and layers. In the future, I would keep trying to add more layers and neurons in order to capture the complex state of the data. Furthermore, I would bin the data even further with reducing the integrity of the dataset.
