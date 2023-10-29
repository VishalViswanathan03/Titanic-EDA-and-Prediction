# Titanic-EDA-and-Prediction
Exploratory Data Analysis on the Titanic dataset and predicting survival using logistic regression model. 
Load Data: The training and testing datasets are loaded from CSV files ("train.csv" and "test.csv") using Pandas.

Data Exploration: Initial data exploration, checking for missing values and displaying the first few rows of the training dataset. 

Data Visualization: Seaborn is used to create bar plots to visualize the relationships between the "Sex" and "Pclass" features and the target variable "Survived."

Handling Missing Values: Missing values are filled in the "Age" column with a placeholder value (-0.5) and creates an "AgeGroup" feature by categorizing ages into groups.

Data Preprocessing: Unecessary columns are dropped ("Ticket," "Cabin," "Fare") and handles missing values in the "Embarked" column by filling them with "S" (the most common value).

Feature Engineering: Titles from the "Name" column are extracted and categorized into common titles (e.g., Mr, Miss) and rare titles. It also converts categorical features like "Sex," "AgeGroup," and "Embarked" into numerical values using Label Encoding.

Machine Learning: The data is prepared for machine learning, separating features and the target variable.Then a logistic regression model is trained.

Generate Predictions: Predictions are generated on the test data and creates a submission file ("result.csv") containing the passenger IDs and their corresponding survival predictions.

Model Evaluation:  The model's performance is evaluated on the training data using accuracy score.
