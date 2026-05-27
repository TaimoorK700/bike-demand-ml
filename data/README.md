# Data Folder

This folder should contain the Bike Sharing Dataset files used in this project.

## Dataset

This project uses the UCI Bike Sharing Dataset, which contains hourly and daily bike rental records from the Capital Bikeshare system, along with weather, seasonal, and calendar-related features.

The main file used in this project is:

`hour.csv`

## Expected Files

After downloading and extracting the dataset, this folder should contain:

- `hour.csv`
- `day.csv`
- `Readme.txt`

The notebooks mainly use `hour.csv` because the project predicts hourly bike-sharing demand.

## How to Get the Data

Download the Bike Sharing Dataset from the UCI Machine Learning Repository:

https://archive.ics.uci.edu/dataset/275/bike+sharing+dataset

After downloading, extract the dataset and place `hour.csv` inside this `data/` folder.

## Notes

The raw dataset is not included directly in this repository to keep the project lightweight and avoid unnecessary data duplication.

The project excludes `casual` and `registered` from the model features because:

`cnt = casual + registered`

Using those columns to predict `cnt` would leak the answer into the model.
