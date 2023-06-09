
# Compass Real Estate Time Series Analysis

Author: Emily Marsh

## Introduction

In the United States, a common investment oppurtunity for personal and commercial investment is real estate. In 2023 the average the average annual return on investment for residential real estate in the United States is 10.6 percent. Commercial real estate averages a slightly lower ROI of 9.5 percent, while REITs average a slightly higher 11.8 percent. There have been recent historical events that have had an impact on this annual return on investment. The housing crash in 2011 as well as the COVID pandemic of 2020 have had outsized impacts on pricing of housing, however a consistent increase over time has made this an area of consistent profits. Compass Real Estate, an real estate brokerage company that specializes in high-margin, luxury homes in upscale markets, has commissioned this project to expand into a new lower cost housing market in order to appeal to a broader group of clients and quicker cash flow.

## Business Objective

Compass Real Estate is interested in investing in lower priced housing, under $300,000, for a smaller but more consistent revenue stream to supplement their luxury housing investments. This will also give the company the chance to expand their client base to more middle class home buyers. However, before investing capitol in this new venture, Compass would like to do analysis into determining the best five zipcodes that provides the biggest chance of profit. Using the dataset, this analysis will provide insight into the five best zip codes for investment as well as the projected profits over the next five years in each zip code. These predictions will be made using Time Series modeling.

## Dataset

The dataset used for this project is a subset of a larger dataset from Zillow, and consists of 14,732 rows and 272 columns. The format of the dataset includes features about RegionID, Region Name (Zipcode), City, State, Metro, County Name, Size Rank, and the average price of houses in the zipcode starting in April of 1994 and ending with April of 2018. Each RegionName/Zipcode is a unique value, while Metro and County Name are not. It is also important to note that the dataset is in a wide format versus a long format. Therefore in order to pass this data into a model, the dataset will need to be reshaped to a long format.

## Data Preparation

A dataset with 14723 rows would require substantial processing power to run through a model. Therefore in order to streamline the process, the dataset will be filtered using the client's budget and the zipcodes that show the greatest return on investment. In order to determine this, the profit of each zip code will be subtracted from the original price of the average property in April of 1996 from the average property value in April of 2018. Due to the client's budget, the available houses will be limited by price, only properties with a value of under $300,000 as of April 2018. Since Compass is a national company, geography is not a limiting factor for investment consideration therefore no geographical constraints will be used to limit the available zipcodes.

## Methods

In order to determine which time series model is appropriate for the data series, four models will be built. Once built, the most accurate time series model will be selected to fine tune and make predictions for final recommendations. The RMSE score will be used as a determinate of which model is the most accurate. The reason the RMSE will be used is that, as an expression of how closely the data points are around the line of best fit, the highest RMSE score shows the most accurate prediction and limits the amount of unpredicted values. This is important since the client wants to as accurately as possible predict future ROI on investment.

## Visualizing Time Series Model Performance

## Conclusions

## Recommendations

## Next Steps

## References

## For More Information

The full analysis and process by which these conclusions were reached can be found in the Jupyter notebook or by reviewing the summary presentation.

For additional questions, contact Emily Marsh: marshemily2@gmail.com

## Repository Structure

|── Data
 
 ├── Images
 
 ├── README.md
 
 ├── PhaseFourFinalProjectPresentation.pdf
 
 └── PhaseFourProject.ipynb
