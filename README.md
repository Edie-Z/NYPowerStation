# Power Plant Combustion Optimization Project: Data Analysis and Visualization

This project aims to optimize the combustion process in power plants by utilizing data analysis and visualization techniques to address nitrogen oxides (NOx) and carbon monoxide (CO) emissions.  
The project includes data preprocessing, visualizations for a feasibility analysis report, and single-step predictions using Long Short-Term Memory (LSTM) models.

The **Long Short-Term Memory (LSTM)** model is a type of recurrent neural network (RNN) designed to capture long-term dependencies in time series data.  
LSTMs are particularly effective for sequential data, where current predictions rely on previous time steps, such as predicting nitrogen oxide emissions over time.

## Project Structure

This project contains the following files:

- **NYDA3_Preprocess.ipynb**: Data Preprocessing and Descriptive Analysis
    - This notebook is responsible for preprocessing the input data, including data cleaning, handling missing values, and performing descriptive statistical analysis.
      It also utilizes visualization techniques to display the distribution of nitrogen oxides and carbon monoxide values while applying filters to handle outliers.
      Additionally, it calculates boiler thermal efficiency.

- **NYDA3_FeasibilityReport.ipynb**: Visual Illustrations for the Feasibility Analysis Report
    - This notebook generates visualizations for the feasibility analysis report, aiding in the understanding of the project's implementation feasibility.
      It includes various graphical representations to support analytical conclusions.

- **NYDA3_LSTM1stepPrediction.ipynb**: Single-Step Prediction Using LSTM
    - This notebook uses a Long Short-Term Memory (LSTM) model to predict nitrogen oxides (NOx) on a single-step basis.
      It includes the data preparation process, the construction of the LSTM model, the loss function, the optimizer, and the prediction steps.

- **DATA3.xlsx**: Input Data File
    - This file contains the raw data collected during the operation of the power plant, including key performance indicators.
        
- **filter.py**: Encapsulated Filtering Code
    - This script provides functions for processing and filtering data, which are called in `NYDA3_Preprocess.ipynb` to remove noise and outliers, ensuring data accuracy.
