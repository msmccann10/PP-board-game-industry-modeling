# **Board Game Prediction**

**Author:** Michael McCann
___

**Project currently underway. Please check back to see the finished results!!**

## Overview
This project looks at two datasets on board game rankings and characteristics as reported on the popular board game website, Board Game Geek. In this project I attempt to find what (if any) characteristics drive game rankings on Board Game Geek and attempt to make a model which will predict the popularity of a given game based on its characteristics. My goals for this project are as follows:
1. Create a regression model which will predict the average user ranking of a game on Board Game Geek.
2. Create a classification model which will predict if a game will break into the top 100 on Board Game Geek (a benchmark by which games are measured in the industry).
3. Create a recommendation engine to recommend games based on user preference/rankings. **This has since been split into its own separate project**

## Business Problem
For this analysis I attempted to address two business seperate but related business problems:
+ A fictional company is looking at multiple proposals for new games and would like to predict which of these games will be popular/successful. They would like to know the projected rankings of these games on Board Game Geek, as well as, what features are most important/predictive of a games popularity.
+ A fictional game store has limitted inventory space and wants to ensure that it is only purchasing merchandise that will be popular and generate sales. To this end the store wants to know if a new game is likely to break into the top 100 games on Board Game Geek, a benchmark they are using for success/popularity.


## Data
### Data Sources
The data for this project comes from two separate datasets loaded onto kaggle. These datasets were cleaned and combined to make a single comprehensive dataset for exploratory data analysis and machine learning. Our data sources are as follows: 
+ [Board Game Geek Rankings](https://www.kaggle.com/datasets/mseinstein/bgg_top2000): A kaggle dataset of the top 5,000 ranked games on Board Game Geek. These rankings are scraped directly from the Board Game Geek website and updated weekly. The data is divided into three CSVs with general information, rankings by game ID, and rankings by game name.

+ [Board Game Database from BoardGameGeek](https://www.kaggle.com/datasets/threnjen/board-games-database-from-boardgamegeek): A kaggle dataset of in-depth board game characteristics for 20,000 games. This dataset was pulled using the Board Game Geek API and is updated quarterly. The data is divided into 9 CSVs containing data on designers, artists, publishers, mechanics, themes, categories, and user rankings.

The original datasets have been stored in this repository and can be found [here](https://github.com/msmccann10/Portfolio/tree/main/board-game-prediction/data). 

The dataset consists of....

### Data Dictionary
| Variable | Description |
| ------   | ----------- |
| Item Identifier | Unique Product ID |
| Item Weight | Weight of the Product |
| Item Fat Content | Whether the Product is Low Fat or Regular |
| Item Visibility | The Percentage of Total Display Area of All Products in a Store Allocated to the Product|
| Item Type | The Category to Which the Product Belongs|
| Item MRP | Maximum Retail Price (list price) of the Product|
| Outlet Identifier | Unique Store ID |
| Outlet Establishment Year | The Year in which the Outlet was Established|
| Outlet Size | The Size of the Outlet in Terms of Ground Area Covered|
| Outlet Location Type | The Type of Area in which the Outlet is Located|
| Outlet Type | Whether the Outlet is a Grocery Store or some sort of Supermarket|
| Item_Outlet_Sales | Sales of the Product in the Particular Outlet.|

### Data Validation
+ **Duplicates:** 
+ **Missing Values** 
  - 
  - 
+ **Inconsistent Data:** 
  - 
  - 

### Caveats and Considerations
Insert caveats/warnings/etc

## Methods
See my [Jupyter Notebook](https://github.com/msmccann10/Portfolio/blob/main/board-game-prediction/Board_Game_Prediction.ipynb) for detailed steps I took to clean and analyze the data. The general steps were as follows:
1. 
2. 
3. 
4. 
5. 

## Results

### Witty Title
Observations and Images

### Witty Title
Observations and Images

### Witty Title
Observations and Images

### Witty Title
Observations and Images
The data provided does not allow us to evaluate for premium space such as end caps or promotional locations. However, based on these findings we suggest further studies evaulate the relationship between sales and premium space to determine if it provides a positive return on investment.


## Machine Learning 
I used four machine learning models to determine which (if any) would help predict future sales. The results were as follows:

| Model             | RSME          | Train R2 | Test R2 |
| ----------------- | ------------- | -------------- | ------------- |
| Dummy / Baseline  | 1678.869      | 0.000          | -0.000        |
| Linear Regression | 1135.226      | 0.568          | 0.543         |
| Decision Tree     | 1145.560      | **0.938**      | 0.534         |
| Bagged Tree       | 1142.236      | **0.938**      | 0.535         |
| Random Forest     | **1097.597**  | 0.623          | **0.586**     |


??? Model performed best... explain

### Feature Importance


## Recommendations
+ 
+ 
+ 

## For More Information
Please review my full analysis in my [Jupyter Notebook](https://github.com/msmccann10/Portfolio/blob/main/board-game-prediction/Board_Game_Prediction.ipynb) or my [presentation - UPDATE LINK WHEN COMPLETE]().

For any additional questions, please contact **Michael McCann**, [**msmccann10@gmail.com**](mailto:msmccann10@gmail.com).
