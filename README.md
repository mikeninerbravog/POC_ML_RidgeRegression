# Machine Learning - Ridge Regression Proof of Concept (POC)

This repository demonstrates how **Ridge Regression** improves predictions by reducing overfitting. The examples focus on two real-world scenarios:

1. **Predicting Real Estate Prices**: Estimating property prices based on features like size, number of rooms, construction year, and distance to the city center.
2. **Forecasting Supermarket Sales**: Predicting product sales based on promotions, weekdays, weather, and special events.

## What is Ridge Regression?

**Ridge Regression** is an improved version of **Linear Regression** that prevents overfitting by applying a penalty to large coefficients. It helps create a more balanced model, particularly when working with many variables.

### Why Use Ridge Regression?
- **Reduces Overfitting**: Ensures that the model does not "memorize" the data but learns patterns effectively.
- **Works Well with Multiple Variables**: Handles datasets with many features efficiently.
- **Provides More Stable Predictions**: Avoids giving excessive weight to irrelevant variables.

## Running on Google Colab

### Step 1: Open the Notebooks in Colab
Click the links below to open the examples directly in **Google Colab**:
- [Predicting Real Estate Prices](https://colab.research.google.com/github/mikeninerbravog/POC_ML_RidgeRegression/blob/master/PocMLSupervisedL_RidgeRegression.ipynb)
- [Forecasting Supermarket Sales](https://colab.research.google.com/github/mikeninerbravog/POC_ML_RidgeRegression/blob/master/PocMLSupervisedL_RidgeRegression.ipynb)

### Step 2: Install Dependencies (if needed)
Google Colab usually comes with required libraries pre-installed. However, if needed, run:
```python
!pip install numpy matplotlib scikit-learn
```

### Step 3: Run the Cells
Each notebook contains explanations, data, and visualizations. Execute the cells in order to train the models and visualize results.

## Example 1: Predicting Real Estate Prices

This model predicts **property prices** based on key real estate factors:

- **Input Features**: 
  - Property size (m²)
  - Number of rooms
  - Construction year
  - Distance from the city center
- **Output**: Predicted property price
- **Comparison**: Standard Linear Regression vs. Ridge Regression

### Notebook Highlights:
- A **Linear Regression model** is first trained, showing potential overfitting.
- A **Ridge Regression model** is applied, demonstrating better generalization.
- A **scatter plot** visualizes the real vs. predicted values for both models.

## Example 2: Forecasting Supermarket Sales

This model predicts **product sales** based on various influencing factors:

- **Input Features**:
  - Promotions
  - Day of the week
  - Weather (temperature)
  - Special events
- **Output**: Predicted number of products sold
- **Comparison**: Standard Linear Regression vs. Ridge Regression

### Notebook Highlights:
- A **Linear Regression model** is tested first, showing how some variables may receive excessive weight.
- A **Ridge Regression model** is trained, preventing extreme weight assignments.
- The **mean squared error (MSE)** is compared between models to evaluate performance.

## Visualizing Results

Each notebook generates a **scatter plot** comparing **Linear Regression** and **Ridge Regression**:
- **Blue dots**: Predictions using Linear Regression.
- **Red dots**: Predictions using Ridge Regression.
- **Dashed black line**: Ideal fit (perfect prediction).
- **Lower MSE in Ridge Regression**: Shows improved generalization.

## Conclusion

**Ridge Regression** is an essential improvement over standard **Linear Regression**, ensuring more reliable predictions by controlling coefficient magnitude. It is widely used in fields like **real estate pricing, sales forecasting, finance, and marketing**.

## License

This project is released under the MIT License.
