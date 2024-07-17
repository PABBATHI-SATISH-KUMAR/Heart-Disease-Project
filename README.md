### Heart Disease Prediction Using Machine Learning: A Logistic Regression Approach

#### Abstract
Heart disease is a leading cause of mortality worldwide, and early prediction can significantly improve patient outcomes. This paper outlines the development of a machine learning model using logistic regression to predict heart disease based on clinical data. The model is trained and validated using a publicly available dataset. A user-friendly web interface is implemented to facilitate real-time predictions and result storage. The effectiveness of the model is evaluated using accuracy metrics, highlighting its potential application in healthcare.

#### Introduction
Heart disease remains a critical health challenge globally, with timely diagnosis being crucial for effective treatment. Machine learning offers promising tools to predict heart disease risk, enabling proactive medical interventions. This study focuses on building a logistic regression model to estimate the likelihood of heart disease, leveraging various clinical attributes.

#### Methodology

**1. Data Collection and Preprocessing**
The dataset used for this project is sourced from the UCI Machine Learning Repository, containing 303 instances with 14 attributes, including age, sex, cholesterol levels, and blood pressure. The target variable indicates the presence of heart disease.

- **Data Loading:** The dataset is loaded using pandas.
- **Data Cleaning:** Missing values are handled, and non-predictive columns are removed.
- **Feature Selection:** Relevant features are selected based on domain knowledge.

**2. Model Development**
Logistic regression, a robust machine learning algorithm for binary classification, is employed.

- **Data Splitting:** The dataset is divided into training (80%) and testing (20%) sets using stratified sampling to maintain class distribution.
- **Model Training:** The logistic regression model is trained with a maximum iteration limit set to 1000.
- **Evaluation Metrics:** Model performance is evaluated using accuracy, with additional metrics like the confusion matrix for deeper insights.

**3. User Interaction and Real-time Prediction**
A web interface is developed using Flask to enable user interaction.

- **Input Features:** Users input clinical data through a web form.
- **Real-time Prediction:** The trained model predicts the likelihood of heart disease based on user input.
- **Result Storage:** Predictions are stored in an SQLite database for future reference.

#### Results
The logistic regression model achieved an accuracy of approximately 85% on the training data and 82% on the testing data. The web interface effectively captures user input and provides real-time predictions, enhancing accessibility for non-technical users.

#### Discussion
The results demonstrate the feasibility of using logistic regression for heart disease prediction. The relatively high accuracy indicates the model's potential utility in clinical settings. The web interface and database integration ensure that the system is user-friendly and capable of storing historical predictions for trend analysis.

#### Conclusion
This study presents a comprehensive approach to predicting heart disease using machine learning. The logistic regression model, combined with a user-friendly web interface, provides an effective tool for early diagnosis and intervention. Future work will explore incorporating more advanced machine learning techniques and larger datasets to further enhance prediction accuracy.
