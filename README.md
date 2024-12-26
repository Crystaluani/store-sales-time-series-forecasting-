# Store-sales-time-series-forecasting-

## Project Overview
This project aims to forecast store sales using a time series dataset. The dataset includes information such as oil prices, holiday events, store details, transactions, and historical sales data. 

The project applies various machine learning models, such as **Linear Regression** and **XGBoost**, to predict sales and evaluate model performance.

## Dataset Details
The dataset consists of the following CSV files:
- `holidays_events.csv`: Information about holidays and events.
- `oil.csv`: Daily oil price data.
- `stores.csv`: Store metadata.
- `transactions.csv`: Number of transactions at each store.
- `train.csv`: Historical sales data for training.
- `test.csv`: Sales data for testing.
- `sample_submission.csv`: Submission format for predictions.

  
## Visual Details
- I created a combined csv file 'visualization_data' to create a more detailed visual using tableau.


## Tools & Libraries
The following tools and libraries were used:
- **Python**: Data analysis and modeling
- **Pandas**: Data manipulation
- **Scikit-learn**: Machine learning models
- **XGBoost**: Advanced regression model
- **Matplotlib & Seaborn**: Data visualization
- **VS Code**: Code editor

## Steps Followed
1. **Data Loading**:
   - All CSV files were loaded and combined using Pandas.

2. **Data Preprocessing**:
   - Handled missing values (e.g., filling missing oil prices with forward fill).
   - Merged datasets on relevant keys such as `date` and `store`.

3. **Exploratory Data Analysis (EDA)**:
   - Visualized sales trends over time.
   - Analyzed relationships between transactions, oil prices, and sales.

4. **Feature Engineering**:
   - Created new features like day, month, and year from the `date` column.
   - Incorporated holiday and oil price data into the training set.

5. **Model Building**:
   - Implemented multiple models:
     - **Linear Regression**: Baseline model with MAE = 451.87
     - **XGBoost** = 318.34
   - Evaluated performance using Mean Absolute Error (MAE).

6. **Results**:
   - The Linear Regression model achieved an MAE of **451.87**, which represents the average prediction error.

## Results
The best model so far (Linear Regression) resulted in:
- **Mean Absolute Error (MAE): 451.87**

## Future Work
- Hyperparameter tuning for Random Forest and XGBoost.
- Exploring advanced time series models like SARIMA or LSTM.
- Incorporating external data (e.g., weather, competition trends).
