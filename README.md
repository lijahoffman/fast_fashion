# fast_fashion

Insights into Cross-Continental Fast Fashion

The following analysis considered the number of inventory items in the Myntra CSV and the number of search results returned using the ASOS API.

Abishai file
1. contains graphs for autcomplete function for ASOS API

2. Myntra csv data analysis



File Fashion_Lija_Update.ipynb contains: 
1. Search results for pink, blue, and green by country, as well as agg statistics for each color across countries. 

2. Analysis of the API search results compared to the merchandise inventory listed in the CSV. Specifically, the number of blue, pink, and green garments relative the neutrals black and white. 

3. Chi-squared significance test of the number of observed ASOS API results for each color compared to the expected number of results (MyIntra color proportions multiplied by the total number of ASOS items). 


Lija Conclusions: 

According to the Myntra CSV, which was last updated at the beginning of 2022, the total number of clothing items of the specified colors (in descending order) were as follows: blue, black, green, white, pink. In contrast, the ASOS API, which was updated in the past month, produced the following ordering of the average number of search results for each color: pink, blue, green, white, black. The increased proportion of pink and green items in the ASOS dataset compared to the Myntra dataset appears to be in line with the colors forecasted to trend after the release of the Myntra dataset. Indeed, a chi-squared test comparing the actual number of ASOS search result for each color to the expected number of search results for each color (calculated by multiplying the color proportions of the Myntra dataset by the total number of ASOS search results), yielded a statistically significant p-value of 0.0, suggesting the observed difference in color proportion was unlikely to be due to random change. 

With respect to the distribution of “trend” color search results across countries, the analyses demonstrated variation in the overall popularity of certain colors, as well as popularity between countries. As previously mentioned, pink was found to have the greatest mean number of search results (2.21e 4), followed by blue (2.00e 4) and green (1.75e 4). While pink was popular across countries (var = 3.77e 7, SD = 6.14e 3), France returned the greatest number of results when entering pink into the search and Germany returned the least. Blue was found to have the greatest variation (6.87e 7) and standard deviation (8.29e 3) in search results, proving to be most popular in Italy and least popular in Spain. Green also displayed variation in the number of search results returned (var = 4.15e 7, SD = 6.44e 3), with the greatest number of results returned in the United States and the fewest number of results returned in Spain. 
