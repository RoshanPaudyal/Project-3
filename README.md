## Project 3: Predicting Customer Purchase Success Rate
### Executive Summary
The objective of this project is to develop a model that can predict the success rate of customer purchases using machine learning techniques. The goal is to provide businesses with insights to optimize their marketing strategies and resource allocation. Three models were explored: Neural Networks, K-Nearest Neighbours (KNN), and Random Forest Classifier. Based on the results, the recommended model is the Random Forest Classifier due to its highest Training Data Accuracy (99.09%) and Test Data Accuracy (89.38%). Feature selection was considered but resulted in lower accuracy scores. The potential application of the model is to optimize marketing strategies and resource allocation to increase sales and revenue.

### Concept
The project leverages variables related to user behaviour, website interactions, and administrative factors to predict customer purchase success rate. The dataset used in the project is taken from UC Irvine's Machine Learning Repository dataset.

### Data Collection, Clean-up, and Exploration
The dataset includes variables such as Page values, Product Related Duration, Exit Rates, Bounce Rates, Product Related, Administrative Duration, Month, Administrative, Region, and Informational Duration. The data was cleaned up by handling missing values, outliers, and data inconsistencies. Exploratory Data Analysis (EDA) was performed to understand the distribution, relationships, and patterns within the dataset. Feature Engineering was also carried out by creating new features or transforming existing ones to enhance model performance. However correlation matrix resulted in lower prediction scores, possibly due to class imbalance. We considered undersampling but due to time constraints and other challenges, we decided to use all the features.

#### Model Building
We built three different models using the following algorithms:

- Neural networks: A deep neural network with several layers. We used Keras with a TensorFlow backend to build the model. The neural network had the highest accuracy on the training data, with a score of 99.09%. However, its performance dropped on the test data, with an accuracy score of 83.35%.

- K-nearest neighbours: An unsupervised algorithm that classifies data based on its proximity to other data points in a given space. We used scikit-learn to build the model. This algorithm had a lower accuracy than neural networks, with a score of 80.04% on the training data and 78.39% on the test data.

- Random forest: A supervised algorithm that builds multiple decision trees and combines their outputs to make predictions. We used scikit-learn to build the model. This algorithm had the highest accuracy on the test data, with a score of 89.38%, and a very high accuracy on the training data as well, with a score of 99.09%.

#### Model Evaluation
We evaluated the performance of each model using the following metrics:

- Precision: measures how often the model correctly predicts a positive class.
- Recall: measures how often the model correctly identifies a positive class.
- F1-score: the harmonic mean of precision and recall.
- AUC-ROC: a measure of the model's ability to distinguish between positive and negative classes.

We used the classification_report function from the scikit-learn library to generate these metrics for each model on both the training and testing sets. The results are as follows:

![image](https://user-images.githubusercontent.com/116679505/237027946-856962a4-6ebc-4769-a32c-f978426d3215.png)



### Approach
The dataset was split into training and testing sets. Each model was trained using the training data, and model performance was evaluated using accuracy metrics. The recommended model is the Random Forest Classifier due to its high Training Data Accuracy (99.09%) and Test Data Accuracy (89.38%). Feature selection was attempted but resulted in lower prediction scores.

### Demo
The functionality and performance of the Random Forest Classifier were showcased in the project. A sample prediction was presented using new input data, highlighting the model's ability to predict the success rate of customer purchases.

### Next Steps
- Utilize the developed model to help businesses optimize their marketing strategy and allocate resources effectively.
- Provide personalized recommendations to improve customer engagement and conversion rates.
- Fine-tune the model by adjusting the parameters and training parameters to optimize effectiveness.
- Continuously monitor and update the model to adapt to changing customer behaviors and market trends.
- Obtain more data to potentially increase the accuracy of scores.
- Explore additional datasets or features that may enhance the model's predictive capabilities.
- Collaborate with businesses to implement the model and measure its impact on sales and revenue.
- Fine-tune the model by adjusting the parameters and training parameters to optimize performance.
### Instructions
The code and instructions for running the project are provided in the repository. The main.py file contains the code for data cleaning, preprocessing, model training, and evaluation. The demo.py file contains the code for showcasing the performance of the Random Forest Classifier. The data folder contains the dataset used in the project.

### Conclusion
The project successfully developed a model to predict the success rate of customer purchases. The Random Forest Classifier outperformed the other models, with a high Training Data Accuracy (99.09%) and Test Data Accuracy (89.38%). The potential application of the model is to optimize marketing strategies and resource allocation to increase sales and revenue.

