# Rainfall Prediction Project

## Module 13 – Assignment 9: Rainfall Prediction

This project is part of the Full Stack Data Science & AI course. It involves building a Linear Regression model using Python to predict rainfall (precipitation) based on historical weather data from Austin, Texas. The analysis includes data cleaning, preprocessing, model training, evaluation, and insightful visualizations.

## Objective

To predict **PrecipitationSumInches** using various weather parameters such as:

- Average Temperature
- Average Humidity
- Dew Point
- Wind Speed
- Visibility
- Sea Level Pressure
  
## Dataset

- **Filename:** `austin_weather.csv`
- **Description:** Contains historical weather data for Austin, Texas.
- **Source:** Provided through course LMS  
- **Target Variable:** `PrecipitationSumInches`


## Tools & Libraries Used

- Python
- Jupyter Notebook
- NumPy
- Pandas
- scikit-learn
- Matplotlib


##  Methodology

### 1. **Data Preprocessing**
- Dropped irrelevant columns: `Events`, `Date`, `SeaLevelPressureLowInches`
- Replaced missing values like `'T'` (Trace) and `'-'` with `0.0`
- Converted all columns to numeric types
- Removed rows with missing data (`NaN`)

### 2. **Feature Selection**
- Independent variables (features): All relevant numeric weather attributes
- Dependent variable (target): `PrecipitationSumInches`

### 3. **Model Building**
- Used `LinearRegression` from `sklearn`
- Trained on the full dataset

### 4. **Model Evaluation**
- Calculated **R² Score** for model performance
- Calculated **Root Mean Squared Error (RMSE)** for prediction error

### 5. **Visualization**
- Precipitation trends over time
- Scatter plots showing relationships between precipitation and other weather parameters

---

## Results

- The Linear Regression model was able to fit the weather data and predict precipitation.
- Model performance metrics were computed and displayed in the notebook.
- Visualizations clearly show how weather attributes influence rainfall levels.

---

## Project Structure
rainfall-prediction-project/

├── austin_weather.csv # Original dataset

├── austin_weather_final.csv # Cleaned dataset (optional)

├── rainfall_prediction.ipynb # Jupyter Notebook with full analysis

└── README.md # Project overview and instructions

##  How to Run

1. Clone the repository or download the ZIP.
2. Open `rainfall_prediction.ipynb` in Jupyter Notebook.
3. Run the cells in sequence to see the full analysis, model training, and plots.



