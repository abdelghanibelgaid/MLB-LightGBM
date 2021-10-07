# MLB Player Digital Engagement Forecasting - LightGBM with Hyperparameter Tuning
LightGBM approach to predict fan engagement with baseball player digital content.

## About
The aim of this competition is to understand the factors that lead to rise & fall in supporter engagement for players. The task is forecasting four different measures of engagement (`target1`, `target2`, `target3`, `target4`) for a subset of MLB players who are active in the 2021 season. Additional information about the competition can be found on the [Kaggle Competition page](https://www.kaggle.com/c/mlb-player-digital-engagement-forecasting).

## Datasets
The data contains a set of static files that do not change with time (`players.csv`, `teams.csv`, `seasons.csv`, `awards.csv`) as well as daily data (`train.csv`) which is grouped by day. When predicting on a given `date`, the model forecast the target variables for the next day (i.e. for `date` d, you're predicting the engagement for day d+1).

`train.csv` - the training set.

`example_test.csv` - an example in the form of the test set that you’ll be evaluated on.

`example_sample_submission.csv` - A sample submission file in the correct format based on the example test set.

`awards.csv` - A collection of awards given out prior to 01/01/2018 (the first date in train.csv).

`players.csv` - Library containing high level information about all MLB players in this dataset.

`seasons.csv` - Information about start and end dates of all seasons in this dataset.

`teams.csv` - Library containing high level information about all MLB teams.

Additonal public datasets were used in the training phase. Further information about the datasets can be found on the [Kaggle Data Description page](https://www.kaggle.com/c/mlb-player-digital-engagement-forecasting/data).

## Model Overview
The model is based on a hyperparameter tuning on LightGBM with an MAE score of 0.933 in the four targets of engagement.

## Contributing
Github issues and pull requests are welcome. Your feedback is much appreciated!

September 2021, Abdelghani Belgaid
