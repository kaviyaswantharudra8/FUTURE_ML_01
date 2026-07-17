# FUTURE_ML_01 - Sales and Demand Forecasting Model

## About This Project
This is my submission for Task 1 of the Future Interns Machine Learning track. I built a Python forecasting model from scratch to predict future monthly store sales using historical retail transaction data. 

When businesses don't know what their future demand looks like, they either overstock inventory (wasting money) or run out of products during peak seasons (losing sales). The goal of this model is to take past sales patterns and turn them into a reliable visual forecast so a business owner can make better decisions on stocking, budgeting, and staffing.

## How I Built It
* **Language & Environment:** Python 3, Jupyter Notebook
* **Data Processing:** I used Pandas and NumPy to clean the raw transaction data, convert date strings into standard datetime objects, and group daily transactions into total monthly revenue.
* **Feature Engineering:** To help the machine learning algorithm understand time, I extracted month and year features and created a "lag feature" (using the previous month's revenue to help predict the current month's sales).
* **Model Used:** I trained a `RandomForestRegressor` from Scikit-Learn using an 80/20 train-test split so I could test the model's accuracy against real unseen data.
* **Visualization:** I used Matplotlib to plot the actual sales against the AI predictions so the results are easy for non-technical users to understand at a glance.

## Results
The model successfully tracked the upward and downward seasonal trends of the store's revenue. I evaluated its performance using Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE). You can check out the generated graph in the `sales_forecast_chart.png` file included in this repository.
