## Dataset description

The time series included in this repository is related to the electricity consumption in Spain from 1 January 2007 at 00:00 to 21 June 2016 at 23:50. It is a time series of 9 years and 6 months with a high sampling frequency (10 minutes), resulting in 497,832 measures in total.

The time series was processed creating a window of 144 lagged values corresponding to one day and a horizon of 24 values corresponding to 4 hours. Thus, the past day is used to predict the next 4 hours. After the preprocessing, we have removed the first 144 rows and the last 24 rows, in order to avoid empty values in the instances.

## Description of files:

- timeseries_raw.csv.zip - The original multivariate time series including energy consumption every 10 minutes.
- dataset_w144_h24.csv - The lagged version of the time series using a window size of 144 values and a prediction horizon of 24 values.
- dataset_w144_targetXX.arff - The lagged version of the time series using a window size of 144 values and a single class for regression at the XX ahead value.
