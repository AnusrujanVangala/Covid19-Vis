
---

# 📊 India COVID-19 Forecasting
This repository contains Python scripts and data to analyze and forecast the spread of the coronavirus (COVID-19) in India using historical data and Prophet time series forecasting.

## 🧾 Overview

The goal of this project is to load and process India's daily reported cases and deaths related to the coronavirus, then train a forecasting model using Facebook's Prophet library to predict future trends. The model outputs forecasts with confidence intervals and plots components such as trends and seasonality.

## 📁 Files Included

| File | Description |
|------|-------------|
| `Covid19Trends.twbx` | Tableau packaged workbook with visualisations of trends and predictions of the model |
| `Untitled.ipynb.txt` | A Jupyter Notebook script containing the core logic for loading data, preprocessing it, training the model, and making predictions. |
| `covid_19_india.csv` | Historical dataset containing daily reported cases and deaths in India (empty in current repo). |
| `covid_forecast.csv` | Output CSV from the Prophet model, including forecasted values and uncertainty intervals. |


## 🔧 Requirements

You'll need to install the following packages if not already installed:

```bash
pip install pandas prophet matplotlib
```

Ensure that the notebook uses Python 3.8 or above due to dependencies on Prophet and Pandas libraries.

## 📈 Features

- Clean and preprocess raw case/death data.
- Train a Prophet model for forecasting.
- Plot forecast results and model components (trend, seasonality).
- Generate cumulative totals for new cases and deaths over time.

## ▶️ How to Run

1. Open the `Untitled.ipynb.txt` file in a Jupyter Notebook environment.
2. Ensure `covid_19_india.csv` contains valid historical data in the required format.
3. Run each cell sequentially to:
   - Load and clean the data.
   - Train the Prophet model.
   - Generate and visualize forecasts.

Alternatively, you can run the script via terminal or Python IDEs like VSCode or Colab.

## 📌 Example Data Format (`covid_19_india.csv`)

The expected format of the input dataset is:

```csv
Date,NewCases,DailyDeaths
2020-01-30,1,0
2020-01-31,1,0
...
```

If the provided `covid_19_india.csv` is empty, you’ll need to source the correct dataset and place it in the working directory.

## 📝 Sample Output

After running the script, the output will include:

- Forecasted total cases and deaths for upcoming days.
- Graphical visualizations showing:
  - Total cases over time.
  - Model components (trend, weekly, yearly).

## 📎 License

MIT License – see LICENSE for more details.

---

### ✅ Acknowledgments

- [Facebook Prophet](https://facebook.github.io/prophet/) – For robust time-series forecasting.
- [Pandas](https://pandas.pydata.org/) – For powerful data manipulation.
- Publicly available datasets used for modeling purposes.

---

