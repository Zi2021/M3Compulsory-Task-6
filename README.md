# M3Compulsory-Task-6
Comment from coding mentor: 
It looks like you've included names, like "Partner, Mr. Austen", in the dataset, which is causing a problem during model training. The error message could not convert string to float occurs because the DecisionTreeClassifier requires numerical data, but it encountered text data that it couldn’t process.

To resolve this, make sure all columns in your training data (X_train) are converted to numeric format. Here’s what to check and do:

- Identify Categorical Columns: Any columns containing names, titles, or non-numeric values should be identified and preprocessed.
- Convert Categorical to Numeric: Use techniques like label encoding or one-hot encoding to transform categorical data into numeric format.
These steps will help ensure the model can work with the data without errors. Once you’ve made these changes, rerun the model to see if it proceeds without issue.
