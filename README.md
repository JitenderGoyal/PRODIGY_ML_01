# House Prices Prediction: Linear Regression

This project aims to predict house prices based on their square footage, number of bedrooms, and bathrooms using a Linear Regression model. The dataset used in this project is provided in a CSV file named "house_data.csv."

## Project Structure

The project follows a structured approach, including data analysis, data preprocessing, feature selection, model training, and performance evaluation. Here is an overview of the key steps taken in the project:

1. **Import Necessary Libraries**: Start by importing essential Python libraries, such as NumPy, Pandas, Matplotlib, and Seaborn, for data analysis and visualization.

2. **Load the Dataset**: Load the dataset from the "house_data.csv" file into a Pandas DataFrame for further analysis.

3. **Data Analysis**:
   - Check the shape of the dataset using `df.shape`.
   - Display the first few rows of the dataset with `df.head()`.
   - View summary statistics of the dataset using `df.describe()`.
   - Check for missing values with `df.isnull().sum()`.
   - Display information about the dataset using `df.info()`.
   - Remove the 'date' column as it's not relevant to the analysis.

4. **Data Preprocessing**:
   - Convert 'bedrooms' and 'bathrooms' columns to integer data types.
   - Identify numerical variables and visualize their correlations with a heatmap.
   - Explore year-related features and their relationship with 'price.'
   - Categorize features as discrete, continuous, or categorical.

5. **Feature Visualization**:
   - Visualize relationships between discrete and continuous variables using bar plots and histograms.
   - Detect and visualize outliers using box plots.
   - Explore categorical variables through bar plots and check unique categories.

6. **Feature Selection**:
   - Select specific columns to keep for model training.
   - Create a heatmap to visualize feature correlations.

7. **Log Transformation**:
   - Apply a log transformation to the 'sqft_living' feature and visualize the distribution.

8. **Pairplot Visualization**:
   - Create a pairplot to visualize relationships between features.

9. **Model Training**:
   - Split the data into training and testing sets using `train_test_split`.
   - Train a Linear Regression model using `LinearRegression` from scikit-learn.
   - Make predictions on the test set and evaluate the model's performance with R-squared.

10. **Model Performance Visualization**:
    - Visualize the regression line and actual data points.
    - Create a residual plot and a histogram of residuals.

11. **Make Predictions on New Data**:
    - Create new data for prediction.
    - Use the trained model to predict the price for the new data.
