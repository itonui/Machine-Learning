# MPG Prediction Using Linear Regression and Gradient Descent

This project involves building and comparing two regression models to predict the miles per gallon (MPG) of cars based on various features such as weight, horsepower, displacement, etc. The models implemented are:

- **Model 1**: A traditional Linear Regression model using Scikit-learn's `LinearRegression` class.
- **Model 2**: A custom Gradient Descent Linear Regression model that uses manually implemented gradient descent optimization.

## Key Sections

### 1. Data Preprocessing
- The dataset is cleaned by handling missing values and normalizing the features using `StandardScaler`.
- Missing values in the `'horsepower'` column are replaced with the median using the `fillna()` function.
- The data is then split into training and test sets.

### 2. Model 1: Linear Regression
- **Model 1** is a traditional linear regression model built using Scikit-learn’s `LinearRegression` class. This model serves as the baseline for comparison.
- The performance of this model is evaluated using:
  - **MSE (Mean Squared Error)**: Measures the average of the squares of the errors.
  - **R-squared**: Represents the proportion of the variance for the dependent variable that's explained by the independent variables.

### 3. Model 2: Gradient Descent Linear Regression
- **Model 2** is implemented from scratch using gradient descent optimization.
- The learning rate and the number of iterations are configurable as hyperparameters, allowing for experimentation and tuning.
- A custom training loop updates the weights and biases using mini-batch gradient descent.
- Model performance is evaluated using MSE and R-squared scores, with hyperparameter tuning for:
  - Learning Rate (`eta`): Determines the step size at each iteration.
  - Number of Iterations: Controls how long the model will keep learning.
  
### 4. Comparison of Models
- Both models are compared based on their **MSE** and **R-squared** scores.
- This comparison evaluates the effectiveness of the manually implemented gradient descent model (Model 2) compared to the traditional linear regression model (Model 1).
- Additionally, the impact of different hyperparameters (learning rate, iterations) on the performance of Model 2 is analyzed.

### 5. Visualization
- A scatter plot compares the **predicted MPG values versus the actual MPG values** for both models.
- Additional scatter plots are used to **visualize the prediction errors** for both models, highlighting how well each model performs across different ranges of the actual data.

### 6. Error Analysis
- Prediction errors are calculated by subtracting the predicted values from the actual values.
- **Scatter plots** are generated to visualize these errors, showing where the models make incorrect predictions and by how much.
  
