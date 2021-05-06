Superconductive Data-X: Making Machine Learning Faster and Accessible For All

The Problem:
Building Machine Learning (ML) model is a very complex, time-consuming and challenging process. Data scientists spend much of their time on data cleaning and preparation. Moreover, they have to experiment on different ML Algorithms and compare all evaluation metrics to obtain the best results. This experimentation process can be lengthy and tedious making the barrier to entry high for ML jobs. Superconductive is aspired to make ML faster and accessible for all individuals and businesses. We built an ML platform to help data scientists quickly create complicated ML pipelines and identify the best model without coding while reducing the model creation time by at least half.  

Solution:
Superconductive offers a low-coded ML platform. The platform was built on many built-in function packages, so users don’t have to code. It streamlines the creation of all ML pipelines by summarizing commonly used methods for EDA, data cleaning, feature transformation and engineering, model building and evaluation. The tool is highly customized because users can make decisions throughout the process leveraging their insight. 

Methods:
Users are guided through each step of the ML and asked to select from various function packages in a user-friendly web environment. First, a user is provided with several data cleaning methods including handling missing values, data type conversion, text cleaning, etc. Next, seven different feature transformation options are provided. Depending on the needs, the user can transform any column by applying the selected method. The tool will then help the user create and identify the best interaction features. The tool is designed to solve both regression and classification problems with algorithms including logistic, KNN, SVM, random forest and decision tree. All models can automatically tune hyperparameters and ensure delivery of the best performance. Finally, the tool visualizes all model performances using various evaluation metrics to enable the user to easily identify the best model. Additionally, the tool uses EDA visualization to help users make more informed decisions along the process. 

Back End Code Structure: Superconductive allows users to build their ML models without coding by offering comprehensive built-in function packages at each ML stage.

The options below under each stage are most commonly used by data scientists. Although covering every scenario in a semester-long project is unrealistic, our packages can easily be extended per user needs in the future. 

I. Upload Dataset: display general information for the dataset including unique value for each column

II. Data Cleaning/Pre-processing: 
A. Handling missing data: visually shows missing data proportions and replace it with a median value of the column or automatically removes the columns that have more than 50% of missing data. (in the future, we can add web interaction to ask user to confirm before removing)
B. Datatype conversion: allows user to convert numerical column into strings or convert string columns into numerical columns.
C. Extraction function: allows user to extract numbers from a string (letter + numbers) or extract letters from a string (letter + numbers). The extracted content will be created as a new feature. 
D. Time stamp: convert time stamp data into new features like year, month, day, day of week, and week. 
E. Cleaning up strings: allows user to clean up string columns by removing html tags, emoticons, and all special characters. 
F. Drop columns: allows users to drop multiple columns. 

III. EDA Visualization:
A. Distribution plot: output a 30-bin distribution plot for a chosen column (for continuous variables, show frequency distribution).
B. Count plot: output a count plot for a chosen column (for discrete variables, show frequency distribution).

IV. Feature Transformation:
A. Fourier transform:  transforms the features from the time domain x(t) to the frequency domain X(w) and stores the real part and imaginary part of the resulting function X(w) into two columns respectively.
B. Get dummies: converts nominal categorical values into 0 or 1 numerical values and replaces the original column. 
C. Labelbinarizer: converts binary nominal categorical values into 0 or 1 numerical values and replaces the original column.
D. Ordinal encoder: encodes ordinal categorical values into numerical values and preserves the rank/level within the categorical values.
E. Log transformation: adds a new log-transformed column to the right-end of the data frame.
F. A bag of word: clean, tokenize, and lemmatize words. Identify maximum 100 different words by counting frequency and turn them into new features.  
G. Word2vec: given a set of texts that contains lists of words, calculates the average feature vector (maximum = 100) and turn them into new features. 

V. Feature Engineering & Selection:
A. Feature normalization: normalization.
B. Feature Scaling: feature scaling for numeric columns only in train and test set.
C. Remove outliers: removes outliers using the box plot distribution chart.
D. Choosing top features: allows user to choose top features based on chi2 best score.
E. Adding top interaction features: adding top interaction features based on linear regression score calculated from numerical features.

VI. EDA for Feature Visualization: visualize correlations and covariance between top 20 features using heat map.

VII. Sanity Check for Data Pipeline: applies profiler from great expectation to audit data quality at each data pipeline. A data quality report will be generated. 

VIII. Train & Validation Split: set up training and validation data sets

IX. ML Models & Evaluations:  for classification problems, the tool offers algorithms including logistic, SVM, KNN, random forest, decision tree which are evaluated using accuracy, precision, F1, recall and confusion matrix; for regression problems, the tool offers algorithms including KNN, random forest, decision tree, linear regression which are evaluated using mean absolute error, mean squared error, and root mean squared error. Hyperparameters are automatically tuned to ensure delivery of the best performance.

X. Visualize Results: helps user visualize and compare evaluation metrics for different models. 

Team Member:
Juan Yu: juan.yu@mba.berkeley.edu
Youn Jo Lee: yjlee@berkeley.edu 
Yu Cheng: yu_cheng@berkeley.edu 
Lucy He: lucyhe@berkeley.edu 
Evelyn Yang: evelyny0922@berkeley.edu
