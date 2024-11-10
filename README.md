# House Price Prediction Using Linear Regression

This project demonstrates a simple linear regression model to predict house prices based on the area of the house.

## Key Concepts

- **Linear Regression**: The model learns a linear relationship between the area (feature) and the price (target). The relationship is represented by the equation:
  
  \[
  y = wx + b
  \]

  where `w` is the slope, `x` is the input feature (house area), `b` is the intercept, and `y` is the predicted target (house price).
  
- **Model Training**: The model is trained using the `.fit(x, y)` method, where `x` is the house area, and `y` is the house price. During training, the model learns the values for `w` (slope) and `b` (intercept).
  
- **Prediction**: Once the model is trained, predictions can be made using the `.predict()` method, which uses the learned values for `w` and `b` to predict house prices for new input values.

## Code Explanation

- **Data Visualization**: A scatter plot is used to visualize the relationship between house area and price. The regression line is plotted on top of this scatter plot to show the best-fit line.

- **Model Training**: The `LinearRegression()` class from scikit-learn is used to train the model. After training, the learned parameters (`w` and `b`) are accessed through `lr.coef_` and `lr.intercept_`.

- **Prediction**: After training, the model can predict the price for a given house area. In this example, the price for an area of 130 square feet is predicted and displayed.

## Training Dataset

The training dataset used for this model consists of the following features:

| Area (X) | Price (y) |
|----------|-----------|
| 121      | 300       |
| 125      | 350       |
| 131      | 425       |
| 141      | 405       |
| 152      | 496       |
| 161      | 517       |

The model uses the area (`X`) as the feature and the price (`y`) as the target to learn the relationship between them.

## Steps to Run

1. **Clone the Repository**

    ```bash
    git clone https://github.com/yourusername/house-price-prediction.git
    ```

2. **Install Dependencies**

    Install the required Python libraries by running the following command:

    ```bash
    pip install scikit-learn matplotlib numpy
    ```

3. **Run the Script**

    Run the script using Python:

    ```bash
    python house_price_prediction.py
    ```

    The script will prompt you to enter a house area, and it will display the predicted price along with a plot of the data and the regression line.

## Expected Output

- A plot showing the relationship between house area and price, with the regression line that best fits the data.
- The predicted price for the given house area will be displayed in the terminal.


