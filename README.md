# neural-network-challenge-2
Module 19 Challenge
## Neural Network Challenge: Employee Attrition and Department Prediction

### Overview
This project aims to predict employee attrition and the department best suited for each employee using a branched neural network. The model will help the HR department make informed decisions about employee retention and department assignments. The project is divided into three main parts:

1. Preprocessing
2. Model Creation, Compilation, and Training
3. Summary and Analysis

### Files
- attrition.ipynb: The Jupyter Notebook containing the implementation of the project.

### Instructions
Part 1: Preprocessing

1. Import the data and view the first five rows: Load the dataset and examine its structure to understand the data.

2. Determine the number of unique values in each column: Identify the unique values in each column to help in selecting features and understanding the data.

3. Create y_df with the attrition and department columns: Extract the target variables for attrition and department.

4. Create a list of at least 10 column names to use as X data: Select at least 10 feature columns for the prediction model, excluding attrition and department columns.

5. Create X_df using your selected columns: Form the features dataset with the selected columns.

6. Show the data types for X_df: Display the data types to ensure they are suitable for model training.

7. Split the data into training and testing sets: Divide the dataset into training and testing subsets to evaluate the model's performance.

8. Convert your X data to numeric data types: Encode categorical data and ensure all features are numeric.

9. Create a StandardScaler, fit the scaler to the training data, and transform both the training and testing data: Standardize the features to have a mean of 0 and a standard deviation of 1.

10. Create a OneHotEncoder for the department column, then fit the encoder to the training data and transform both the training and testing data: One-hot encode the department target variable.

11. Create a OneHotEncoder for the attrition column, then fit the encoder to the training data and transform both the training and testing data: One-hot encode the attrition target variable.

### Part 2: Create, Compile, and Train the Model

1. Find the number of columns in the X training data: Determine the input dimension for the neural network.

2. Create the input layer: Define the input layer without using a sequential model since there will be two branched output layers.

3. Create at least two shared layers: Add shared hidden layers to the neural network.

4. Create a branch to predict the department target column: Add a hidden layer and an output layer for the department prediction branch.

5. Create a branch to predict the attrition target column: Add a hidden layer and an output layer for the attrition prediction branch.

6. Create the model: Combine the branches to form the complete model.

7. Compile the model: Compile the model using appropriate loss functions, optimizers, and metrics.

8. Summarize the model: Display the model summary to verify its structure.

9. Train the model using the preprocessed data: Train the model on the training data.

10. Evaluate the model with the testing data: Assess the model's performance on the testing data.

11. Print the accuracy for both department and attrition: Output the accuracy metrics for both predictions.

### Part 3: Summary

Answer the following questions:

1. Is accuracy the best metric to use on this data? Why or why not?

    - Discuss whether accuracy is appropriate for evaluating the model's performance and suggest alternative metrics if necessary.

2. What activation functions did you choose for your output layers, and why?

    - Explain the choice of activation functions for the output layers and their relevance to the prediction tasks.

3. Can you name a few ways that this model could be improved?

    - Suggest potential improvements to enhance the model's performance and reliability.
