**Superconductive**

**[The Problem]**:

Building Machine Learning (ML) model is a very complex, time-consuming and challenging process. Data scientists spend much of their time on data cleaning and preparation. Moreover, they have to experiment on different ML Algorithms and compare all evaluation metrics to obtain the best results. This experimentation process can be lengthy and tedious making the barrier to entry high for ML jobs. Superconductive is aspired to make ML faster and accessible for all individuals and businesses. We built an ML platform to help data scientists quickly create complicated ML pipelines and identify the best model without coding while reducing the model creation time by at least half.  

**[Solution]:**

Superconductive offers a low-coded ML platform. The platform was built on many built-in function packages, so users don’t have to code. It streamlines the creation of all ML pipelines by summarizing commonly used methods for EDA, data cleaning, feature transformation and engineering, model building and evaluation. The tool is highly customized because users can make decisions throughout the process leveraging their insight. 

**[Superconductive_final.py]:**

Superconductive_final.py is the streamlit API written in python with streamlit modules. This displays the each of the sections for the application. User can download our Superconductive.py and start building their data pipeline. The platform is a very user-friendly and users can simply go over the specific sections [refer to the Code Structure below for more information] and choose methods they want to apply as well as the columns that they want to apply to. 

**[Data]:**

This folder contains Titanic CSV file for user to explore and test how Superconductive works. Titanic contains a variety of datatypes, which our low coded machine learning can apply various data transformations and feature transformation methods.

To get started, user should upload their csv file to the drop box. Then Superconductive will show user a high level overview of their dataset and produces a missing data proportions heat map. It will automatically drop the columns that have more than 50% of missing values and replace the other missing values with a median value. 

**[Code Structure]**

**[Data Cleaning/Pre-processing]:**

User should follow the instructions on web and input values accordingly. After each method is applied, a new header for the dataset will be generated for user to review. Ignore the warinings on web if there is any and select the method you need.  

- Convert Data Type: allows user to convert numerical column into strings or convert string columns into numerical columns.

- Extract Numbers From A String: allows user to extract numbers from a string (letter + numbers).The extracted content will be created as a new feature. 

- Extract Letters From A String :extract letters from a string (letter + numbers). The extracted content will be created as a new feature. 

- String Clean-up: allows user to clean up string columns by removing html tags, emoticons, and all special characters. 

- Drop Columns: allows users to drop multiple columns. 

**[EDA Visualization]:**

- Distribution plot: output a 30-bin distribution plot for a chosen column (for continuous variables, show frequency distribution).

- Count plot: output a count plot for a chosen column (for discrete variables, show frequency distribution).

**[Feature Transformation]:**

Transforms the features from the time domain x(t) to the frequency domain X(w) and stores the real part and imaginary -part of the resulting function X(w) into two columns respectively. Depending on the needs, the user can transform any column by applying the selected method. The tool will then help the user create and identify the best interaction features.

- Get dummies: converts nominal categorical values into 0 or 1 numerical values and replaces the original column. 
 
- Label binarizer: converts binary nominal categorical values into 0 or 1 numerical values and replaces the original column.

- Ordinal encoder: encodes ordinal categorical values into numerical values and preserves the rank/level within the categorical values.

- Log transformation: adds a new log-transformed column to the right-end of the data frame.

- A bag of word: clean, tokenize, and lemmatize words. Identify maximum 100 different words by counting frequency and turn them into new features.  

- Word2vec: given a set of texts that contains lists of words, calculates the average feature vector (maximum = 100) and turn them into new features. 

**[Feature Engineering & Selection]:**

- Best features:  Displays 20 top features based on chi2 best score

- Plot Distribution: Displays distribution of a feature to aid user choosing a value for remove outliers

- Remove outliers: removes outliers using the box plot distribution chart.

- Top Interaction: adding top interaction features based on linear regression score calculated from numerical features.

- Drop Column: Drop column

**[EDA for Feature Visualization]:**
Visualize correlations and covariance between top 20 features using heat map.

**[Train & Validation Split]:** 
Set up training and validation data sets

- Feature scaling - Normalization: normalization.

- Feature scaling - Standard Scaler: feature scaling for numeric columns only in train and test set.

**[ML Models & Evaluations]**:  

The tool is designed to solve both regression and classification problems with algorithms including logistic, KNN, SVM, random forest and decision tree. All models can automatically tune hyperparameters and ensure delivery of the best performance. Finally, the tool visualizes all model performances using various evaluation metrics to enable the user to easily identify the best model. Additionally, the tool uses EDA visualization to help users make more informed decisions along the process. 

- for classification problems, the tool offers algorithms including logistic, SVM, KNN, random forest, decision tree which are evaluated using accuracy, precision, F1, recall and confusion matrix; 

- for regression problems, the tool offers algorithms including KNN, random forest, decision tree, linear regression which are evaluated using mean absolute error, mean squared error, and root mean squared error. Hyperparameters are automatically tuned to ensure delivery of the best performance.

**[Visualize Results]**: 
helps user visualize and compare evaluation metrics for different models. 
