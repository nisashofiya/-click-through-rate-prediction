# Click Through Rate Prediction

## Project Backround

With the advent of technology and the internet, there are more opportunities for businesses to reach a wider audience than any physical medium has achieved in the past. However, this also brings new challenges in assessing how well these advertisements perform on a larger scale. The click-through rate is a useful gauge and measurement to evaluate the success of an online campaign for a particular website, product, or service. This project aims to determine which features we should focus on to improve the performance of our advertisements. It seeks to answer fundamental questions about what factors affect the success of an advertisement.

## Objective

1. What factors influence hotel booking cancellations?
2. How accurate is the hotel booking cancellation prediction model?

## Exploratory Data Analysis (EDA)

In the EDA phase, we analyze the Click-Through Rate (CTR) based on various factors to understand their impact on user engagement. The following analyses are performed:

### Click-Through Rate Based on Time Spent on Site

- **Objective**: Examine how the amount of time users spend on the site correlates with the CTR.
- **Analysis**: Explore patterns and relationships between time spent on the site and the likelihood of users clicking through.

### Click-Through Rate Based on Daily Internet Usage

- **Objective**: Investigate the impact of users' daily internet usage on their CTR.
- **Analysis**: Analyze how varying levels of internet usage influence the likelihood of clicks.

### Click-Through Rate Based on Age

- **Objective**: Assess how age affects the CTR.
- **Analysis**: Determine if certain age groups have higher or lower CTR and identify any age-related trends.

### Click-Through Rate Based on Income

- **Objective**: Explore the relationship between users' income levels and their CTR.
- **Analysis**: Analyze how different income brackets impact the likelihood of clicking through.

### Click-Through Rate Based on Country & Continent

- **Objective**: Analyze CTR based on geographic factors, including countries and continents.
- **Analysis**: Group countries by continent and examine regional variations in CTR to identify geographic trends and factors.

### Click-Through Rate Based on Gender

- **Objective**: Investigate how gender affects the CTR.
- **Analysis**: Examine whether different genders exhibit variations in CTR and identify any gender-related patterns.

### Click-Through Rate Based on Day Category

- **Objective**: Analyze CTR based on the category of the day (e.g., weekday vs. weekend).
- **Analysis**: Determine if there are differences in CTR between different days of the week or specific day categories.

## Feature Engineering

Based on the insights gained from EDA, feature engineering is performed to enhance the dataset with relevant features that capture these relationships, improving the model's ability to predict CTR. Key aspects of feature engineering include:

- **Categorizing by Continent**: Grouping countries into continents to analyze regional variations.
- **Timestamp and Day Category**: Creating features that capture the relationship between timestamps and day categories (e.g., converting timestamps into day categories such as weekdays or weekends) to assess how time-related factors influence CTR.

## Model Selection

After performing Exploratory Data Analysis (EDA) and feature engineering, we evaluate various models to determine the most effective one for predicting Click-Through Rate (CTR). The following model has been selected based on its performance metrics:

### LightGBM Model

The LightGBM model demonstrates strong performance with the following metrics:

- **Accuracy**: 0.82
- **F1 Score**: 0.81
- **Precision**: 0.82
- **Recall**: 0.80
- **AUC**: 0.82

**Performance Analysis**:

- **Accuracy**: The model correctly classifies 82% of the data.
- **F1 Score**: With a score of 0.81, the model achieves a good balance between precision and recall.
- **Precision**: The model has a precision of 0.82, indicating that 82% of positive predictions are correct.
- **Recall**: The recall of 0.80 shows that the model correctly identifies 80% of actual positives.
- **AUC**: An AUC of 0.82 suggests that the model is highly effective at distinguishing between positive and negative classes.

The high AUC value indicates that the LightGBM model performs well in distinguishing between the classes, providing robust overall performance. The balance between precision and recall further ensures that the model is effective at accurately classifying the data.
