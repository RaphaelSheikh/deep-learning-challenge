
For this part of the assignment, you’ll write a report on the performance of the deep learning model you created for Alphabet Soup.

The report should contain the following:

Overview of the analysis: Explain the purpose of this analysis.

Results: Using bulleted lists and images to support your answers, address the following questions:

*Data Preprocessing*

1.  What variable(s) are the target(s) for your model?
- The target variable is the 'IS_SUCCESSFUL' column in the application_df dataframe.

2.  What variable(s) are the features for your model?
- The feature variables consist of all columns in application_df, excluding the 'IS_SUCCESSFUL' column, which was removed from the original dataframe.

3.  What variable(s) should be removed from the input data because they are neither targets nor features?
- The 'EIN' and 'NAME' columns were dropped because they were not used as target or feature variables in the dataset.

*Compiling, Training, and Evaluating the Model*

1.  How many neurons, layers, and activation functions did you select for your neural network model, and why?
- In the initial attempt, I used 8 hidden nodes for layer 1 and 5 hidden nodes for layer 2 — these values were random guesses to serve as a starting point for further adjustments in the next iteration.

2.  Were you able to achieve the target model performance?
- I was unable to reach the target model accuracy of 75%.

3.  What steps did you take in your attempts to increase model performance?
- I modified the model by adding more layers, removing additional columns, increasing the number of hidden nodes, and changing the activation functions for each layer in an effort to improve model accuracy.

Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.

Overall, the deep learning model achieved approximately 73% accuracy in predicting the classification problem. Higher prediction accuracy could likely be achieved by improving the correlation between inputs and outputs, which can be done through more thorough data preprocessing and exploring different activation functions, followed by iterative tuning of the model.