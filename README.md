# Financial-Forecasting-Frontier-Distributed-ML
**Description:** Developed a PySpark machine learning model to predict whether bank customers would subscribe to a term deposit. Performed data preprocessing, feature engineering, and classification using Logistic Regression and Random Forest, then compared models using Accuracy, Precision, Recall, F1 Score, and confusion matrix analysis.


Overview
In the modern banking sector, the ability to efficiently process, analyze, and draw insights from vast volumes of data is crucial. Banks and financial institutions generate and collect extensive data, including customer demographics, transaction histories, market trends, and more. This data, when effectively analyzed, can lead to improved customer service, risk management, marketing strategies, and overall operational efficiency.

Project Background
The banking industry faces challenges in managing and utilizing large datasets due to the volume, variety, and velocity of data. Traditional data processing methods often fall short in providing timely insights and handling real-time data streams. With the advent of distributed computing and machine learning technologies, banks now have the opportunity to harness these large datasets to make informed decisions, predict market trends, and enhance customer experiences.

Dataset Overview
age: Age of the individual (integer).
job: Job type (object/string).
marital: Marital status (object/string).
education: Education level (object/string).
default: Indicates if the individual has credit in default (object/string).
balance: Account balance (integer).
housing: Indicates if the individual has a housing loan (object/string).
loan: Indicates if the individual has a personal loan (object/string).
contact: Type of communication contact (object/string).
day: Last contact day of the month (integer).
month: Last contact month of the year (object/string).
duration: Last contact duration, in seconds (integer).
campaign: Number of contacts performed during this campaign for this client (integer).
pdays: Number of days that passed by after the client was last contacted from a previous campaign (integer, '-1' means client was not previously contacted).
previous: Number of contacts performed before this campaign and for this client (integer).
poutcome: Outcome of the previous marketing campaign (object/string).
y: Indicates if the client has subscribed to a term deposit (object/string).
Project Goal
The primary goal of this project is to demonstrate how distributed machine learning can transform banking data into actionable insights. Using the "bank.csv" dataset, students will explore various aspects of distributed computing, from data storage and querying to predictive analytics and real-time data processing. The project aims to simulate a real-world banking data environment, offering insights into customer behavior, identifying key trends, and facilitating data-driven decision-making.

📝 Conclusion of the Project  

> Conclusion:  
> In this project, machine learning models were developed to predict whether a bank customer would subscribe to a term deposit. The data was preprocessed and divided into training and testing datasets. Two classification algorithms, Logistic Regression and Random Forest, were trained and evaluated using Accuracy, Precision, Recall, F1 Score, and actual-versus-predicted classifications.

> Logistic Regression performed better than Random Forest, achieving 89.52% accuracy and an F1 score of 87.83%, compared with 88.47% accuracy and an F1 score of 83.90% for Random Forest. Therefore, Logistic Regression was selected as the better-performing model among the two.

> However, the confusion matrix revealed a significant class imbalance, with both models struggling to identify customers belonging to the positive class (1). This indicates that further improvements such as class weighting, resampling, threshold tuning, and hyperparameter optimization could improve the model's ability to identify potential subscribers.
