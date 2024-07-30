# neural-network-challenge-2
![Screenshot 2024-07-30 at 7 06 30 PM](https://github.com/user-attachments/assets/43852766-52cf-49d0-a19d-62cb29052e02)

## Duane Anglin

# Overview
Instructions:

	1.	Create a neural network for HR to predict employee turnover.
	2.	Predict whether employees are likely to leave the company.
	3.	Predict the department that best fits each employee.
	4.	Use a branched neural network to predict these two columns.

Part 1: Preprocessing

First, import the data and display the first five rows to inspect it. Determine the number of unique values in each column. Create a y_df containing the attrition and department columns. Next, select at least 10 column names to use as X data, excluding the attrition and department columns, and create an X_df using these selected columns, displaying their data types. Split the data into training and testing sets. Convert the X data to numeric data types by fitting encoders to the training data and transforming both the training and testing data. Create a StandardScaler, fit it to the training data, and transform both the training and testing data. Additionally, create and fit a OneHotEncoder for the department column, transforming both the training and testing data, and repeat this process for the attrition column.

Part 2: Create, Compile, and Train the Model

First, find the number of columns in the X training data. Create the input layer, ensuring not to use a sequential model since there will be two branched output layers. Then, create at least two shared layers. For the first branch, which predicts the department target column, use one hidden layer and one output layer. Similarly, for the second branch, which predicts the attrition target column, use one hidden layer and one output layer. After setting up the branches, create and compile the model, then summarize it. Train the model using the preprocessed data and evaluate it with the testing data. Finally, print the accuracy for both the department and attrition predictions.

# References
Chat GPT, Kalvin Anglin, Jaidev Kler, Solutions examples from class.
