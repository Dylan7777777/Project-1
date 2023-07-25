## Data Cleanup
The raw data file is up on our Resources folder in Github. The raw data contained real estate listings in the Eastern region for 16 states and Puerto Rico.
The data set has moved from over 600,000 in its raw format to a little over 6000 after dropping rows with numerous duplicates and those with no values for house size, bedrooms and acreage. 
Data cleanup was fairly straight forward except for the zip code which was imported as a float.
In some cases the zip code was 3 digits or 4 digits and had to be converted to a 5 character string we used the help of a function courtesy Jezrael on stackoverflow.
The cleaned data was exported to the Output folder which you can see in GitHub

## Real Estate Analysis
we imported the cleaned csv file into a dataframe. 
we created a graph showing the average price of homes for all the states (average_property_price)
we created a correlation coefficient matrix of price, house size, number of bedrooms and acreage. 

### Individual State Analysis 
we left out New Hampshire, Vermont and Virgin islands from any individual state analysis as they had just 4, 3 and 1 observation respectively.
for each state - we created individual scatter plot graphs for House size vs house price - Connecticut house prices showed the most correlation with House size r-squared of .63 (price_vs_size_ct)
for each state - we also created individul scatter plot graphs for no. of bedrooms vs house price - Rhode Island was most correlated with a moderate r-squared of .44 (rhodeisland_bedroom_vs_price)
We created a plot and whisker graph for the states (box_plot_states) It waas evident that there were a lot of outliers in most of the states except Delaware.
For the state of Massachusetts we created a scatter plot graph for location (longitude and latitude) and attached a color bar to show variation of house prices by color.
For Massachusetts we also plotted the listings (relatively few 62) on a map of Massachusetts which for the most part displays to us that location matters.

####
Finally, We sorted values by price for the whole dataset and have mapped that data (expensive_map_listings_by_price.png) 
This last chart along with the Massachusetts map listing reiterates the phrase "location location location " and the data confirms the phrase. 
