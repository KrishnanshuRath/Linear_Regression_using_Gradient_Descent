# Linear_Regression_using_Gradient_Descent

## Simple Linear Regression Using Gradient Descent (No Library Support)

## Overview
This project demonstrates the implementation of **Simple Linear Regression** using **Gradient Descent** without relying on external libraries like Scikit-Learn. The regression model is trained on a dataset containing **100 instances** of an independent (predictor) variable and their corresponding dependent (response) variable.

## Features
- **Manual Gradient Descent Implementation**: No external libraries used.
- **Mean Squared Error (MSE) Loss Function**: Optimized using gradient descent.
- **Regression Line & Scatter Plot**: Visualizes the best-fit line against the data points.
- **Cost vs Iteration Plot**: Analyzes convergence over **50 epochs** with three different learning rates (**0.005, 0.5, and 5**).
- **Comparison of Different Gradient Descent Techniques**:
  - **Batch Gradient Descent (BGD)**
  - **Stochastic Gradient Descent (SGD)**
  - **Mini-Batch Gradient Descent (MBGD)**
  - Cost vs Iteration plots compared for all three methods.

 ## Dataset
- Contains **100 data points**.
- Features:
  - **X (Independent Variable) – Predictor**
  - **Y (Dependent Variable) – Response**

## Gradient Descent Implementation
The model parameters (**θ₀ and θ₁**) are optimized using **Gradient Descent**, with the following approach:
1. Initialize parameters to zero.
2. Compute the hypothesis function:

     ![image](https://github.com/user-attachments/assets/104e6f70-75dd-4c2d-b76e-2ab0fda6961c)

4. Compute the cost function using Mean Squared Error (MSE):  

      ![image](https://github.com/user-attachments/assets/c5103412-66c2-43b0-b97a-228e8d7abf40)

5. Update parameters iteratively:

      ![image](https://github.com/user-attachments/assets/8e679b33-0c76-48b4-89b6-02586e72fdcf)


7. Stop when convergence criteria are met (cost function change < **1e-6**).

## Observations
- The learning rate significantly impacts convergence speed:
  - **0.005**: Converges slowly but steadily.
  - **0.5**: Converges quickly without oscillations.
  - **5**: Diverges due to large step sizes.
- **BGD vs SGD vs MBGD**: Cost function behavior compared for all three methods.

 ## Visualizations
- **Regression Line & Scatter Plot**: Displays fitted regression line.
- **Cost vs Iteration Plots**:
  - Compared for three learning rates.
  - Compared across **BGD, SGD, and MBGD**.

## Requirements
- Python 3.x
- Numpy (for data import and data manipulation)
- Matplotlib (for visualization)

