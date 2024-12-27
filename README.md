Cyber Security Physical System Threat Identification

Cybersecurity for physical systems involves protecting critical infrastructure, industrial control systems, and other tangible assets from cyber threats. The integration of digital technologies in various sectors has increased efficiency but also exposed these systems to potential vulnerabilities. Identifying and mitigating threats to physical systems is crucial to ensure the continued operation and safety of critical infrastructure

Data Selection and Preprocessing: The script begins by loading a dataset from a CSV file (UNSW_NB15.csv) using the Pandas library. The dataset is then examined by displaying the first 15 rows.

Handling Missing Values: The script checks for missing values in the dataset and prints the sum of missing values for each column.

Label Encoding: The 'attack_cat' column is label-encoded using scikit-learn's LabelEncoder to convert categorical labels into numerical format. Additionally, label encoding is applied to the 'proto', 'service', and 'state' columns.

Data Splitting: The dataset is split into training and testing sets using sci-kit-learn's train_test_split function.

Feature Extraction - PCA (Principle Component Analysis): Principle Component Analysis (PCA) is applied to reduce the dimensionality of the dataset to 40 components.

Classification - LSTM (Long Short-Term Memory): The script defines an LSTM model using TensorFlow's Keras API. The LSTM model is trained on the training data with a specified architecture. The model is compiled using the mean absolute error (MAE) loss function and the Adam optimizer.

Performance Analysis: The accuracy of the LSTM model is evaluated and printed.

Comparison with Logistic Regression (LR): Logistic Regression is applied separately, and its accuracy is evaluated and printed. A comparison bar graph is generated to visualize the accuracies of the LSTM and Logistic Regression models.

Prediction: The script performs predictions using the logistic regression model on the test data and prints whether each instance is classified as 'Normal' or 'Cyber Attack'. Comparison Graph:

A bar graph is created to visually compare the accuracy of the LSTM model and Logistic Regression. 

![LSTM Bar Graph](https://github.com/user-attachments/assets/ffec7570-17da-4a1b-84eb-9cda8bf5abe9)


