# Health Insurance Cross-Sell-Prediction

## Project Overview
This project aims to predict the potential of cross-selling vehicle insurance to customers who have health insurance. Utilizing various machine learning models, the project identifies customers who are more likely to purchase vehicle insurance. This is crucial for devising effective marketing strategies and improving customer engagement.

## Dataset
The dataset contains information about health insurance customers, such as age, gender, region, previously insured status, vehicle age, vehicle damage history, and whether the customer is interested in vehicle insurance (response).

# Health Insurance Cross-Sell Prediction

## Project Overview
This project aims to predict the potential of cross-selling vehicle insurance to customers who have health insurance. Utilizing various machine learning models, the project identifies customers who are more likely to purchase vehicle insurance. This is crucial for devising effective marketing strategies and improving customer engagement.

## Dataset Description
The dataset includes the following variables:

### Training Data
| Variable              | Definition                                                                                         |
|-----------------------|----------------------------------------------------------------------------------------------------|
| id                    | Unique ID for the customer                                                                         |
| Gender                | Gender of the customer                                                                             |
| Age                   | Age of the customer                                                                                |
| Driving_License       | 0: Customer does not have DL, 1: Customer already has DL                                           |
| Region_Code           | Unique code for the region of the customer                                                         |
| Previously_Insured    | 1: Customer already has Vehicle Insurance, 0: Customer doesn't have Vehicle Insurance              |
| Vehicle_Age           | Age of the Vehicle                                                                                 |
| Vehicle_Damage        | 1: Customer got his/her vehicle damaged in the past. 0: Customer didn't get his/her vehicle damaged|
| Annual_Premium        | The amount customer needs to pay as premium in the year                                            |
| Policy_Sales_Channel  | Anonymized Code for the channel of outreaching to the customer                                     |
| Vintage               | Number of Days, Customer has been associated with the company                                      |
| Response              | 1: Customer is interested, 0: Customer is not interested                                           |

### Test Data
The test data includes the same variables as the training data, except for the `Response` variable.

## Models Used
- RandomForestClassifier
- LinearDiscriminantAnalysis
- GaussianNB
- DecisionTreeClassifier
- KNeighborsClassifier
- ExtraTreesClassifier

Each model was evaluated based on accuracy, precision, recall, and F1-score to determine its effectiveness in predicting the likelihood of customers purchasing vehicle insurance.

## Methodology
1. **Data Preprocessing**: Included handling missing values, encoding categorical variables, and splitting the dataset into training and validation sets.
2. **Exploratory Data Analysis (EDA)**: Conducted to understand the dataset's characteristics.
3. **Model Training and Evaluation**: Various models were trained and evaluated on their performance metrics.
4. **Model Selection**: Models were compared based on accuracy, precision, recall, and F1-score to select the best model for the task.

## Key Findings
- **RandomForestClassifier** showed the best overall performance, making it the most suitable model for this task.
- **LinearDiscriminantAnalysis** had the highest recall, useful for maximizing the identification of interested customers.
- **ExtraTreesClassifier** also performed well and can be considered as an alternative.

## Usage
The models can be used to predict whether a health insurance customer would be interested in vehicle insurance. This can aid in targeted marketing and personalized customer engagement strategies.

## Authors
- Mustafa Noman
