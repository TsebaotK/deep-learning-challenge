# deep-learning-challenge


1.	Overview of the analysis: Explain the purpose of this analysis.
        This analysis is aimed to provide a tool to the non-profit organization Alphabet Soup for selecting applicants for funding with the best chance of success in their venture. 
        It predicts whether applicants will be successful if funded by Alphabet Soup, based on recorded data from 34,000 organizations that have received funding from Alphabet Soup over the years, 

2.	Results: Using bulleted lists and images to support your answers, address the following questions:
    •	Data Preprocessing
        o	What variable(s) are the target(s) for your model?
                From the application data frame, the column "IS_SUCCESSFUL" is considered the target.

        o	What variable(s) are the features for your model?
                From the application data frame, all columns except for "EIN," "NAME," & "IS_SUCCESSFUL" is considered as the featured for my model.

        o	What variable(s) should be removed from the input data because they are neither targets nor features?
                The "EIN" & "NAME" columns are considered neither targets nor features and are removed from the input data, which 

•	Compiling, Training, and Evaluating the Model
    o	How many neurons, layers, and activation functions did you select for your neural network model, and why?
            In the first AphabetSoupCharity file, I considered two hidden layers with 80 and 30 neurons and the "relu" activation to be suitable parameters for the data set and used it to create a neural network model
 
    o	Were you able to achieve the target model performance?
            I could not achieve the targeted 75% model performance with this model. The accuracy was 0.725 & loss was 0.55.
 
    o	What steps did you take in your attempts to increase model performance?
              i.	To increase the model performance, I removed additional columns, 'STATUS' and 'SPECIAL_CONSIDERATIONS.'
             ii.	I increased the cutoff value of the 'APPLICATION_TYPE' and 'CLASSIFICATION' to decrease the number of unique values.
            iii. 	I created an additional bin to the "ASK_AMT" column with 8747 unique values. 
             iv.	I increased the hidden layers to three and used 100, 80, and 50 neurons.
              v.	I used "ReLu" activation of the first hidden layer and checked the other two layers with the "LeakyReLU" and "tanh."
             vi.	I checked the performance by increasing and reducing the number of epochs to train the regimen.
             

3.	Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.
            The deep learning model uses neurons to train the selected portion of the data to determine the success of applicants for funding with the best chance of success in their venture. However, the methodology chosen could not achieve the targeted 75% model performance. 
            As the deep learning model could not achieve the expected performance, we should check other methods to see which best model for the data. Decision Trees, Random Forests, Support Vector machines, and Gradient Boosting Machines are some of the methods. 
            The Random Forests model is the next methodology to model this data. This model handles large datasets with high dimensionality and ample training examples. It builds multiple decision trees and combines their predictions to improve accuracy and reduce overfitting. 



