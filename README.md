# Deep Learning
![image](https://github.com/user-attachments/assets/94d31e39-d8ea-45b0-bf7e-f329419d5e98)

# Background
The nonprofit foundation Alphabet Soup is seeking a tool to help select applicants for funding who have the highest likelihood of success in their ventures. Using my knowledge of machine learning and neural networks, I’ll work with the features provided in the dataset to build a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

Alphabet Soup’s business team has provided me with a CSV containing data on over 34,000 organizations that have previously received funding. This dataset includes various columns capturing metadata about each organization, such as:

* EIN and NAME: Identification columns
* APPLICATION_TYPE: Alphabet Soup application type
* AFFILIATION: Affiliated sector of industry
* CLASSIFICATION: Government organization classification
* USE_CASE: Purpose for the requested funding
* ORGANIZATION: Type of organization
* STATUS: Current operational status
* INCOME_AMT: Income classification
* SPECIAL_CONSIDERATIONS: Special considerations for the application
* ASK_AMT: Amount of funding requested
* IS_SUCCESSFUL: Indicator of whether the funding was used effectively

# Instructions

                                  Step 1: Preprocess the Data

Using my knowledge of Pandas and scikit-learn’s **`StandardScaler()`**, I'll preprocess the dataset to prepare for the next step, where I'll compile, train, and evaluate the neural network model.

First, I'll upload the starter file to Google Colab. Using the information provided in the Challenge files, I'll follow the instructions to complete the preprocessing steps.

I'll start by reading in the **`charity_data.csv`** file into a Pandas DataFrame. Then, I'll identify the following in the dataset:

What variable(s) are the target(s) for my model?
What variable(s) are the feature(s) for my model?

I'll drop the **`EIN`** and **`NAME`** columns as they won't be useful for the model.

Next, I'll determine the number of unique values for each column. For columns that have more than 10 unique values, I'll identify the number of data points for each unique value.

Based on that information, I'll use the number of data points to choose a cutoff point to combine "rare" categorical variables into a new value called "Other," and then check if the replacement was successful.

Afterward, I'll use **`pd.get_dummies()`** to encode the categorical variables.

I'll then split the preprocessed data into a features array **`x`** and a target array **`y`**. Using these arrays and the **`train_test_split`** function, I'll split the data into training and testing datasets.

Finally, I'll scale the training and testing features datasets by creating a **`StandardScaler`** instance, fitting it to the training data, and using the **`transform`** function to apply the scaling.

                                  Step 2: Compile, Train, and Evaluate the Model

Using my knowledge of TensorFlow, I'll design a neural network, or deep learning model, to create a binary classification model that can predict whether an Alphabet Soup-funded organization will be successful based on the dataset's features. I'll need to consider how many input features there are before determining the number of neurons and layers for my model. Once that’s done, I’ll move on to compiling, training, and evaluating the model to calculate its loss and accuracy.

I’ll continue using the Google Colab file where I completed the preprocessing steps from Step 1.

Here’s how I’ll proceed:

First, I'll create the neural network model by assigning the number of input features and determining the number of nodes for each layer using TensorFlow and Keras.
I'll create the first hidden layer and select an appropriate activation function (like ReLU).
If needed, I'll add a second hidden layer with an appropriate activation function.
Then, I’ll create the output layer using a suitable activation function, such as sigmoid, since this is a binary classification problem.
Once the layers are defined, I’ll check the structure of the model to ensure everything is set up correctly.
After setting up the model:

I'll compile it, selecting the appropriate loss function (binary crossentropy for binary classification) and optimizer (like Adam).
I'll train the model using the training data.
Additionally, I'll create a callback function to save the model's weights every five epochs.

Once the training is complete, I'll evaluate the model using the test data to check its loss and accuracy.

                                  Step 3: Optimize the Model
Using my knowledge of TensorFlow, I'll optimize my model to achieve a target predictive accuracy higher than 75%.

To optimize the model, I can use any or all of the following methods:

1. Adjust the Input Data: I'll ensure that no variables or outliers are causing confusion in the model. This might involve:

* Dropping more or fewer columns based on their relevance.
* Creating more bins for rare occurrences in categorical columns to better group the data.
* Increasing or decreasing the number of values for each bin to ensure a balanced representation.

2. Modify the Neural Network Structure:

* I can add more neurons to a hidden layer to increase the model's capacity to learn.
* If necessary, I'll add more hidden layers to allow the model to capture more complex patterns in the data.

3. Experiment with Activation Functions: I'll try different activation functions for the hidden layers to see if a different approach leads to better performance.

4. Adjust Training Regimen:

* I may add or reduce the number of epochs during training, depending on how well the model is learning and whether it’s overfitting or underfitting.
By systematically applying these optimization techniques, I'll work towards improving the model's predictive accuracy to exceed the 75% target.

                                  Step 4: Write a Report on the Neural Network Model

# References

* IRS. Tax Exempt Organization Search Bulk Data Downloads. (https://www.irs.gov/)

* What is Machine Learning? (https://www.datacamp.com/blog/what-is-machine-learning)

* Machine Leaning Tutorial (https://www.geeksforgeeks.org/machine-learning/)

* What is a neural network? (https://www.cloudflare.com/learning/ai/what-is-neural-network/)

* Reinforcement Learning with Neural Network (https://www.baeldung.com/cs/reinforcement-learning-neural-network)
