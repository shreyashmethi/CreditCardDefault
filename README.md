# Credit Card Default Prediction

This project aims to predict credit card defaults using machine learning models. It uses a dataset containing information about credit card holders, including their payment history, bill amounts, and demographic features. The goal is to build models that can accurately predict whether a credit card holder will default on their payment next month.

## Dataset

The dataset used for this project is called UCI_Credit_Card.csv. It contains the following columns:

- `LIMIT_BAL`: Credit card limit
- `SEX`: Gender (1 = male, 2 = female)
- `EDUCATION`: Education level (1 = graduate school, 2 = university, 3 = high school, 4 = others)
- `MARRIAGE`: Marital status (1 = married, 2 = single, 3 = others)
- `AGE`: Age in years
- `PAY_0` to `PAY_6`: Payment status from April to September (-1 = on time, 1 = one month late, 2 = two months late, ..., 9 = nine months or more late)
- `BILL_AMT1` to `BILL_AMT6`: Bill amount from April to September
- `PAY_AMT1` to `PAY_AMT6`: Amount paid from April to September
- `default.payment.next.month`: Target variable indicating whether the customer defaulted on their payment next month (1 = yes, 0 = no)

## Requirements

- Python (version 3.6 or later)
- Jupyter Notebook
- pandas
- numpy
- scikit-learn
- matplotlib

## Usage

1. Clone the repository:

```bash
git clone https://github.com/shreyashmethi/CreditCardDefault.git
```

2. Navigate to the project directory:

```bash
cd CreditCardDefault
```

3. Launch Jupyter Notebook:

```bash
jupyter notebook
```

4. Open the `Credit_Card_Default.ipynb` notebook.

5. Run the notebook cells to execute the code.

## Implementation Details

The code in the notebook follows these steps:

1. Data loading and exploration: The dataset is loaded into a pandas DataFrame, and some initial exploration is performed to understand the data structure.

2. Data preprocessing: The dataset is prepared for model training by handling missing values, encoding categorical variables, and splitting it into input features and target variable.

3. Feature selection: A subset of relevant features is selected based on their correlation with the target variable. Scatter matrix plots are generated to visualize the relationships between selected features.

4. Model training and evaluation: Three machine learning models are implemented and evaluated for credit card default prediction:
   - Stochastic Gradient Descent Classifier (SGDClassifier)
   - Logistic Regression
   - Linear Support Vector Classifier (LinearSVC) and Support Vector Classifier (SVC) with a polynomial kernel

## Results

The performance of the models on the testing set is evaluated using accuracy scores. Here are the results obtained:

- Stochastic Gradient Descent Classifier: 0.803
- Logistic Regression: 0.8255
- Linear Support Vector Classifier: 0.8163
- Polynomial Support Vector Classifier: 0.8253


## References

[1] Dataset: [UCI Credit Card Default Payment](https://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients)

[2] scikit-learn documentation: [https://scikit-learn.org/](https
