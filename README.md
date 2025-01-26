# Weather-Data-Analysis-and-Forecasting
This project involves analyzing and forecasting weather data using a dataset named GlobalWeatherRepository.csv. The goal is to clean the data, perform exploratory data analysis (EDA), detect and handle outliers, and apply forecasting models to derive actionable insights.

## Features
- **Data Cleaning**: Handling missing values, outliers, and normalization.
- **EDA**: Statistical summaries, boxplots, and seasonal decomposition.
- **Forecasting**: ARIMA model implementation with performance evaluation.
- **Insights**: Seasonal trends, air quality analysis, and actionable recommendations.

## Dataset
The dataset used for this project is `GlobalWeatherRepository.csv`, which includes:
- `last_updated`: Datetime information.
- `temperature_celsius`: Recorded temperatures.
- `air_quality_PM2.5`: Air quality index values.
- `precip_mm`: Precipitation in millimeters.

## Why ARIMA?
ARIMA was chosen over other models (e.g., Facebook Prophet) for the following reasons:
- Well-suited for univariate time series data with regular intervals.
- Greater control through explicit parameters (p, d, q).
- Superior performance in terms of Mean Absolute Error (MAE) and RMSE on this dataset.

## Project Structure
```
├── data
│   ├── GlobalWeatherRepository.csv  # Input dataset
├── notebooks
│   ├── analysis.ipynb               # Jupyter Notebook with full analysis
├── outputs
│   ├── visualizations               # Folder for generated plots
├── README.md                        # Project documentation
├── requirements.txt                 # Python dependencies
├── src
│   ├── data_cleaning.py             # Data preprocessing scripts
│   ├── forecasting.py               # ARIMA model implementation
│   ├── visualization.py             # Functions for generating visualizations
```

## Requirements
- Python 3.8+
- Libraries:
  - pandas
  - numpy
  - matplotlib
  - seaborn
  - statsmodels
  - scikit-learn

Install dependencies with:
```bash
pip install -r requirements.txt
```

## Usage
1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/weather-forecasting.git
   ```
2. **Navigate to the directory**:
   ```bash
   cd weather-forecasting
   ```
3. **Run the analysis**:
   Open `notebooks/analysis.ipynb` and execute the cells in a Jupyter Notebook environment.

## Key Results
- **Seasonality**: Temperature exhibits monthly cycles, while air quality shows irregular trends.
- **Forecast Accuracy**: ARIMA achieved high accuracy with low MAE and RMSE values.
- **Actionable Insights**: Dynamic thresholds for air quality monitoring and resource planning recommendations.

## PM Accelerator Mission
> By making industry-leading tools and education available to individuals from all backgrounds, we level the playing field for future PM leaders. This project aligns with the mission by employing advanced methodologies and tools for impactful decision-making.

## Contributing
Contributions are welcome! If you have suggestions or improvements, feel free to create a pull request.
