🚗 Auto Import Price Prediction using Machine Learning

This project focuses on building a machine learning regression model to predict the price of imported cars based on their specifications such as horsepower, engine size, body style, and fuel type. The goal is to help automobile companies, importers, and customers estimate fair market values for cars based on their features.

🧭 Overview

The automobile market is highly competitive and dynamic, with pricing influenced by multiple technical and design factors. Manual estimation of car prices can lead to inconsistencies and bias.
By using data-driven regression models, this project aims to automate the process of predicting car prices accurately based on their physical and performance parameters.

📊 Dataset Description

Dataset Source: UCI Machine Learning Repository — Automobile Dataset

Key Features:
| Feature           | Description                               |
| ----------------- | ----------------------------------------- |
| `symboling`       | Risk factor of the car (insurance rating) |
| `fuel-type`       | Type of fuel (gas/diesel)                 |
| `aspiration`      | Type of aspiration used in the car        |
| `num-of-doors`    | Number of doors                           |
| `body-style`      | Type of car body (sedan, hatchback, etc.) |
| `drive-wheels`    | Type of drive (fwd, rwd, 4wd)             |
| `engine-location` | Position of engine                        |
| `wheel-base`      | Distance between front and rear wheels    |
| `engine-size`     | Engine capacity in cubic centimeters      |
| `horsepower`      | Power produced by the engine              |
| `peak-rpm`        | Engine revolutions per minute             |
| `price`           | Target variable (car price)               |
⚙️ Workflow

Data Loading and Cleaning

Loaded dataset and inspected structure.

Handled missing and inconsistent data.

Feature Engineering

Encoded categorical variables using Label Encoding and One-Hot Encoding.

Normalized numerical features for uniform scale.

Exploratory Data Analysis (EDA)

Visualized relationships between engine size, horsepower, and price.

Identified highly correlated features.

Model Building

Tested multiple regression models:

Linear Regression

Decision Tree Regressor

Random Forest Regressor

Gradient Boosting Regressor

Model Evaluation

Evaluated using R² Score, Mean Absolute Error (MAE), and Root Mean Squared Error (RMSE).

🧠 Best Model

The Random Forest Regressor performed the best with high predictive accuracy and robustness to noise.
It effectively captured the nonlinear relationships between car features and price.

Top Contributing Features:

Engine Size

Horsepower

Drive Wheels

Curb Weight

📈 Results
| Model             | R² Score | Remarks                    |
| :---------------- | :------- | :------------------------- |
| Linear Regression | 0.85     | Good baseline model        |
| Decision Tree     | 0.89     | Interpretable but overfits |
| **Random Forest** | **0.94** | Best performing model      |
| Gradient Boosting | 0.92     | Strong generalization      |

Key Insights:

Higher engine size and horsepower strongly increase price.

Diesel cars tend to be priced higher on average.

Luxury body styles (convertible, sedan) command premium pricing.

🚀 Future Enhancements

Add new features like mileage, year, and brand reputation.

Deploy as a Streamlit/Flask web app for real-time predictions.

Implement model optimization using GridSearchCV and XGBoost.

Integrate API for real-world car data.

🧰 Tech Stack

Python

Pandas, NumPy, Matplotlib, Seaborn

Scikit-learn

Jupyter Notebook
