# Finding Charity Donors

This project aims to build a machine learning model that helps a fictitious charity organization, CharityML, identify potential donors based on demographic data. The goal is to predict whether an individual makes more than $50,000 annually, in order to maximize the charity's donation yield while minimizing the number of letters sent to potential donors.

## Table of Contents

- [Project Overview](#project-overview)
- [Technologies Used](#technologies-used)
- [Data](#data)
- [Model Evaluation](#model-evaluation)
- [Results](#results)
- [Feature Importance](#feature-importance)
- [Conclusion](#conclusion)

## Project Overview

CharityML is a fictitious charity located in Silicon Valley, and the goal of this project is to assist the charity in finding the best candidates for donations. By analyzing demographic data (e.g., age, education, occupation, etc.), we are using supervised learning models to predict which individuals are more likely to donate based on whether their annual income is greater than $50,000.

## Technologies Used

- Python
- Jupyter Notebook
- Scikit-learn
- Pandas
- Matplotlib
- Seaborn

## Data

The dataset used in this project is `census.csv`, which contains demographic data about individuals, such as age, education level, occupation, and income. The main goal of the project is to predict whether an individual earns more than $50,000 annually based on these features.

## Model Evaluation

To evaluate the performance of different machine learning models, we implemented and compared various supervised learning algorithms: Gaussian Naive Bayes, AdaBoost, and Random Forest. Each model's performance was assessed using accuracy and F1 score metrics.

## Results

The best-performing model was the **AdaBoost** classifier. This model was chosen based on both its computational cost and its performance in identifying potential donors.

## Feature Importance

During the project, we also evaluated the feature importance of various demographic features to understand which variables were most important for predicting an individual's income. The following five features were identified as the most relevant:

1. Education num comes in the first place as it directly impacts the type of the job which in turn influences income.
2. Age, since it reflects a prolong job experience, and more job experience usually results in advancements in the career and hence, a higher income.
3. Hours per week: the more of working hours results in a higher income.
4. Capital gain, since it can indicate additional income sources beyond regular wages, often associated with individuals who have accumulated wealth or invested income.
5. Marital status is included as a socio-economic factor that can influence income patterns and financial goals, albeit indirectly.

## Conclusion

By using supervised learning techniques, we were able to develop a model capable of predicting whether an individual is likely to donate to CharityML based on demographic features. The model can be used to send targeted mailings to individuals who are more likely to donate, improving the efficiency of the charity’s outreach efforts.
