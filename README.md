Sea Level Predictor

This project is part of the Data Analysis with Python certification from freeCodeCamp.

In this project, global average sea level change data since 1880 is analyzed and visualized. Using Pandas, Matplotlib, and SciPy, linear regression is applied to predict sea level rise through the year 2050 based on historical trends.

📌 Dataset Overview

The dataset (epa-sea-level.csv) contains global average absolute sea level change from 1880 to 2014 provided by the US Environmental Protection Agency (EPA):

Year: Year of measurement (1880–2014)

CSIRO Adjusted Sea Level: Cumulative sea level changes in inches adjusted by CSIRO

Lower Error Bound & Upper Error Bound: Statistical error ranges

NOAA Adjusted Sea Level: Sea level adjustments provided by NOAA

🛠️ Tasks & Methodology

Import Data: Read the dataset using Pandas.

Scatter Plot: Create a scatter plot using Year on the x-axis and CSIRO Adjusted Sea Level on the y-axis.

Line of Best Fit (All Data):

Use scipy.stats.linregress to calculate the slope and y-intercept for the entire dataset (1880–2014).

Project the trend line through the year 2050.

Line of Best Fit (Recent Data):

Filter data starting from the year 2000 to present.

Calculate a new line of best fit to predict sea level rise through 2050 based on accelerated recent rates.

Plot Customization:

Title: Rise in Sea Level

X-Axis Label: Year

Y-Axis Label: Sea Level (inches)

🚀 Setup & Execution

1. Install Dependencies

Ensure you have Python installed along with the required libraries:

pip install pandas matplotlib scipy


2. Run Main Script

Make sure epa-sea-level.csv, sea_level_predictor.py, main.py, and test_module.py are in the same folder, then execute:

python main.py


📁 File Structure

├── epa-sea-level.csv       # Historical sea level dataset
├── sea_level_predictor.py  # Plotting and regression logic
├── main.py                 # Execution script
├── test_module.py          # freeCodeCamp unit tests
└── README.md               # Project documentation
