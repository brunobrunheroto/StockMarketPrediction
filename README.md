# Stock Market Prediction

<p>Stock Market Prediction is a project done to investigate which machine learning models that can be used to predict stock market prices.</p>

## <ins>Goals</ins>

<p>Investigate and test different machine learning models can be used to predict stock market prices.</p>

## <ins>Objectives of the project</ins>

- Understand the Dataset and cleanup unnecessary features (if required).
- Compare different algorithms for the same problem.
- Show technical scores: R2, RMSE, etc.

## <ins>Strategic plan of action</ins>

1. Frame the problem.
2. Get the Data.
3. Data Cleaning (Removal of unnecessary features).
4. Explore the Data.
5. Prepare the Data (Preprocessing and feature selection).
6. Train the ML Algorithm (Linear Regression).
7. Evaluate using technical scores.

## <ins>Experiment protocol</ins>

- The dataset was divided into training and testing parts in the ratio 80:20, that means 80% of the database will be used for training and 20% for testing.
- The attributes considered for the prediction were the 'volume_obv' and 'volume_adi' indicators. Because all data has been ordered in order of collection, datetime increases increasingly, so instead of using datetime as variable in prediction, the pandas library row index was used, which facilitates calculations in code and decreases execution time. 
- There was a need to pre-process the data, because:
  * The dataset contains an unnamed column, which works as an index, but the pandas library already generates an index automatically when using a dataset, so this column is unnecessary and has been discarded. 
  * The TwelveData platform sends the 5000 most recent data rows collected. the database starts with the last data collected and ends with the oldest 5000°, so it was necessary to reverse the order of the database.

- There was no need to delete data, because all rows contain all attributes, that is, there are no null values in the dataset.
- The metrics for evaluating the results were the coefficient of determination and the root of the mean quadratic error, commonly used to determine regression error.


## <ins>Technologies</ins>

- Python.
<p>Made on Google Colab.</p>

## <ins>How to use </ins>

- Download the "StockMarketPrediction.ipynb" file on this repository and import it on google colab.
- Download the Dataset at "https://drive.google.com/file/d/1e0HUmU2TOZ83guxo5hz1inl1I1rCIMM9/view" and import it on the "sample_data" folder on google colab.
- Run it.

## <ins>Credits</ins>

<p> The ideia to work on this project was shared by the teacher of Artificial Intelligence at Facamp, Carlos Caetano.</p>
