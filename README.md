E-Commerce Sales Forecasting

This project uses 36 months of historical sales data from an electronics company to forecast the next 6 months. The project checks stationarity, handles monthly outliers, analyzes trends and seasonality, and compares SARIMA and XGBoost models using RMSE. The selected model is then used to generate the final sales forecast with 95% prediction intervals.

Data Source: https://www.kaggle.com/datasets/samuelcortinhas/time-series-practice-dataset

How to Run
1. Clone the repository
git clone https://github.com/urham-m/predictive-sales-forecasting.git
2. Go into the project folder
cd predictive-sales-forecasting
3. Create and activate a virtual environment

Windows:

python -m venv .venv
.\.venv\Scripts\Activate.ps1

Mac/Linux:

python3 -m venv .venv
source .venv/bin/activate
4. Install dependencies
pip install -r requirements.txt
5. Run the notebook

Open forecasting_project.ipynb in Jupyter Notebook or VS Code and run the cells from top to bottom.

The notebook prepares the data, tests stationarity, handles outliers, performs decomposition, tunes SARIMA, trains XGBoost, compares the models, and generates the 6-month forecast.

Forecast results are saved in outputs/forecast.csv, and visualizations are saved in outputs/.