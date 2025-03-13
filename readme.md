# Car Sales Data Cleaning and Analysis

This project will cover data cleaning, data analysis and storing data on motherduck using a simple 3 table star schema.

The dataset was provided by a kind human from reddit to be used as an exercise.

## Reporting

The reporting tool to be used will be Evidence and the sample site can be seen [here](https://krtmlry.github.io/car_sales_evidence_repo/).


## Notebooks

1. **data_cleaning.ipynb** - this notebook contains the data cleaning process and the loading process of clean data to motherduck

2. **data_visualization.ipynb** - this notebook contains the sql queries used for creating the analysis report on evidence.


## Directories

1. **dataset** - contains raw and clean excel and csv files of car sales dataset.

2. **img** - contains image for entity relationship diagram.

3. **notebooks** - contains notebooks used for data cleaning and data exploration


## Fact and Dimension tables

This dataset is quite small and I simplified the fact and dimension tables in to three tables.

The entity relationship diagram can be seen under `img` directory named `erd.png`.

1. `dim_dealers` - contains all details about dealers
2. `dim_models` - contains all details about car models
3. `car_sales_clean` - fact table containining facts for each sale records.
4. `car_sales_records` - a table produced for analysis where all facts(id) are replaced by actual values and the date column is extracted into individual parts.


## Data storage

The data is processed locally and then stored at motherduck.






