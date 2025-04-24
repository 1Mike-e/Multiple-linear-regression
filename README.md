# Multiple Linear Regression on 50 Startups Dataset

This project demonstrates how to apply **Multiple Linear Regression** using Python and the `scikit-learn` library to predict startup profits based on various factors such as R&D spending, administration costs, marketing spend, and the state where the company operates.

## Dataset

The dataset used is `50_Startups.csv`, which includes 50 observations with the following columns:

- **R&D Spend** (float)
- **Administration** (float)
- **Marketing Spend** (float)
- **State** (categorical)
- **Profit** (float) — Target variable

## Project Workflow

1. **Import Libraries**  
   The code imports `numpy`, `matplotlib`, and `pandas` for data manipulation and visualization.

2. **Load Dataset**  
   The dataset is read using `pandas.read_csv()`. The features (`X`) and target variable (`y`) are extracted.

3. **Encode Categorical Data**  
   The `State` column (categorical) is encoded using one-hot encoding via `ColumnTransformer`.

4. **Split Dataset**  
   The dataset is split into training and test sets using `train_test_split` with an 80/20 ratio.

5. **Train the Model**  
   A `LinearRegression` model is trained using the training data.

6. **Predict and Compare Results**  
   The model predicts profits on the test set, and the predicted results are compared with actual values.

## Prerequisites

Install required libraries:

```bash
pip install numpy pandas matplotlib scikit-learn

