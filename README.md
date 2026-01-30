Retail-Demand-Forecasting-ARIMA

This project is designed to forecast daily retail sales across various product families using the ARIMA time series model, a well-known statistical forecasting approach. Developed in Python, the application allows users to interactively select a store and product family, generate future demand forecasts, and visualize trends to aid inventory planning and supply chain decisions.

🎯Project Objective

The main goal of this project is to create an end-to-end time series forecasting system that predicts future sales from real-world retail data, helping businesses improve demand forecasting and stock management.

-What I Learned

By working on this project, I developed practical experience in:

Analyzing and preparing time series data

Identifying stationarity and applying differencing techniques

Performing the Augmented Dickey-Fuller (ADF) test

Building and tuning ARIMA models using the statsmodels library

Visualizing historical trends and forecasted values

Writing clean, modular, and interactive Python code

Exporting results such as plots and forecast data to files

Overall, this project strengthened my understanding of data science concepts, statistical modeling, and Python programming.

🧩 Core Concepts Covered

Time Series Forecasting

Stationarity and Differencing

Augmented Dickey-Fuller (ADF) Test

ARIMA (AutoRegressive Integrated Moving Average)

Data Filtering and Indexing

Visualization using Matplotlib

Saving forecasts and plots for further analysis

🔄 Project Workflow

Load and preprocess the retail sales dataset

Display available store numbers and product families

Take user input for selected store and family

Filter and sort the sales data by date

Perform ADF test and apply differencing if required

Train an ARIMA(1,1,1) forecasting model

Predict sales for the next 30 days

Generate and save sales and forecast visualizations

Export forecast results to a CSV file

⚙️ Technologies Used

Python

Pandas – data manipulation and handling

Matplotlib – data visualization

Statsmodels – ARIMA model implementation

NumPy – numerical computations

📁 Dataset

Source: Kaggle – Store Sales Time Series Forecasting

File Used: train.csv

Key Columns:

date

store_nbr

family

sales

📊 Example Run & Outputs

To run the project, execute:

python forecasting.py


You will be asked to:

View the list of available stores and product families

Enter a store number (e.g., 10)

Choose a product family (e.g., HARDWARE)

After execution, the script will:

Test the data for stationarity using the ADF test

Apply differencing when necessary

Train an ARIMA(1,1,1) model

Forecast sales for the upcoming 30 days

Save and display the following outputs:

✅ Raw Sales Plot

Visualizes historical daily sales for the selected store and product family.

✅ Forecasted Sales Plot

Shows the 30-day forecast plotted alongside recent actual sales values.

✅ Forecast CSV Output

The forecast is saved as a CSV file named:

forecast_store<store>_<family>.csv


Example:

forecast_store10_hardware.csv

Date	Forecasted_Sales
2017-08-16	95.67
2017-08-17	94.02
...	...
🚀 How to Run the Project
1. Install Required Libraries
pip install pandas matplotlib statsmodels

2. Add the Dataset

Make sure train.csv is placed in the same directory as forecasting.py.

3. Execute the Script
python forecasting.py

📌 Final Notes

This project effectively connects theoretical time series concepts with real-world implementation. It demonstrates the complete forecasting pipeline—from data exploration and preprocessing to model training, prediction, and visualization—making it a valuable addition to a data science portfolio.
