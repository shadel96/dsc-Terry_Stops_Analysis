# Seattle Terry Stop Data Classification Models and Analysis

##### Author: Spencer Hadel
***
## Overview

In order to h_________________________________

## Data
This analysis utilizes over_____ of data from [terry stopsssss.csv](./data/_______.csv). This data was collected from ____ from 2014-2015, and included the following features:

* `id` - Unique identifier for a house
* `date` - Date house was sold
____ etc

## Methods
This anaylsis first cleans the data present in ______ to remove null values, outliers, and oddities. It then explores the relationship between each of the features on house price, creating visualizations to better understand the effect of these features. 

Next, it preprocesses the data, including normalizing the data so that the model can be properly trained on varying ranges of data, and dividing categorical features into useable variables.

![](./img/corr_heatmap.png)

Finally, the analysis creates multiple JASKLKAGNKALGJLKGMKGL:L: Linear Regression models in order to find the best fitting model. By splitting the data into training and testing sets (75% and 25% of the original dataset, respectively), the best regression model will be able to assess house value and which features add or subtract from that value, according to it's training data.

## Results
NgjkaNLKALGNGKLNASKGLNLKNKL
The analysis revealed a few key points about house sale prices in the area. First of all, we can see clearly what most houses in the area are priced at with a simple distribution plot.

![](./img/price_distribution.png)

This shows us that most houses in King County are valued below $1 million. Additionally, we can see what features have a strong correlation with house value overall, such as square footage, quality of view, number of bed and bathrooms, and whether the property is on a waterfront.

![](./img/price_v_sqft_living.png)
![](./img/price_v_view.png)
![](./img/price_v_bedrooms.png)
![](./img/price_v_bathrooms.png)
![](./img/price_v_waterfront.png)

Finally, we successfully created a model which can correctly predict house sale prices based on this data with about 66% accuracy. This makes it a fantastic baseline for the new company's incentive to create a more data driven approach to its sales. The model works using the following information:

![](./img/model_coef.png)

This breaks down how the model utilizes each piece of information in the data. The intercept score indicates that the model assumes a baseline price for each house to be $976,799 (which holds true to our observation of price distribution of houses in King County), and the model adds or subtracts value from the data per unit of each feature listed by the number alongside it. These numbers are not to be interpreted as directly correlating with house value, but rather indicate the inner workinds of the final predictive linear regression model. 

## Conclusion
The reality is that there is a very broad range of factors that can influence any individual house sale. That being said, there are a multitude of ways we could explore futher. Features like rating, view, and condition could use more exploration, since they are based on arbitrary human concepts. Features like whether or not a house was renovated, or even when it was renovated, also don't necessarily hold value if the type of renovations remain unknown.

Additionally, early phases of the analysis show some correlation of price vs location, which deserves further investigation along with data on the King County area, such as highway locations, points of interest, and the economic status of neighborhoods.

![](./img/price_v_loc.png)

All in all, the model is a decent start to assess house cost, and could be used by the new real estate company to develop a baseling understanding. With additional reseaerch into more particulars of the data, and perhaps another investigation into houses based solely on location, a new analysis could create an even more precise findings to bettern inform the company's decisions.

## More Information
The full analysis can be found in three Jupyter Notebooks: The [Data Cleaning](./kc_data_cleaning.ipynb), [Exploring and Preprocessing](./kc_preprocessing_exploring.ipynb), and [Modeling](./kc_data_modeling.ipynb) phases. Further business conclusions can be found in the [presentation](./kingCounty_pres.pdf).

## Repository Structure

```
├── data
├── img
├── README.md
├── kc_data_cleaning.ipynb
├── kc_data_modeling.ipynb
└── kc_preprocessing_exploring.ipynb
└── kingCounty_pres.pdf
```
