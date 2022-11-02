# Insights into Cross-Continental Fast Fashion

The following analysis considered the number of inventory items in the Myntra CSV and the number of search results returned using the ASOS API.


## Scripts

### Abishai file
1. contains graphs for autcomplete function for ASOS API

2. Myntra csv data analysis


### File Fashion_Lija_Update.ipynb contains: 
1. Search results for pink, blue, and green by country, as well as agg statistics for each color across countries. 

2. Analysis of the API search results compared to the merchandise inventory listed in the CSV. Specifically, the number of blue, pink, and green garments relative the neutrals black and white. 

3. Chi-squared significance test of the number of observed ASOS API results for each color compared to the expected number of results (MyIntra color proportions multiplied by the total number of ASOS items). 


### File Group Project.ipynb Contains: 
Search results for staple piece (Jeans, T-shirts, Sneakers, and sweaters) and search results for fast fashion trends (Leather, Cargo, Overalls, and Animal Print). 


## Conclusions
#### * Note: the following conclusions reflect the API results returned at the time of execution. 


### Lija Conclusions: 

According to the Myntra CSV, which was last updated at the beginning of 2022, the total number of clothing items of the specified colors (in descending order) were as follows: blue, black, green, white, pink. In contrast, the ASOS API, which was updated in the past month, produced the following ordering of the average number of search results for each color: pink, blue, green, white, black. The increased proportion of pink and green items in the ASOS dataset compared to the Myntra dataset appears to be in line with the colors forecasted to trend after the release of the Myntra dataset. Indeed, a chi-squared test comparing the actual number of ASOS search result for each color to the expected number of search results for each color (calculated by multiplying the color proportions of the Myntra dataset by the total number of ASOS search results), yielded a statistically significant p-value of 0.0. 

With respect to the distribution of “trend” color search results across countries, the analyses demonstrated variation in the overall popularity of certain colors, as well as popularity between countries. As previously mentioned, pink was found to have the greatest mean number of search results (2.21e 4), followed by blue (2.00e 4) and green (1.75e 4). While pink was popular across countries (var = 3.77e 7, SD = 6.14e 3), France returned the greatest number of results when entering pink into the search and Germany returned the least. Blue was found to have the greatest variation (6.87e 7) and standard deviation (8.29e 3) in search results, proving to be most popular in Italy and least popular in Spain. Green also displayed variation in the number of search results returned (var = 4.15e 7, SD = 6.44e 3), with the greatest number of results returned in the United States and the fewest number of results returned in Spain. 



### Kevin Conclusion:

It is important to note that the following countries were chosen as a result of having dedicated ASOS websites. These countries were United States, France, Germany, Australia, Italy, and Spain. Thus, these countries would give one better insight on the popularity of a particular style or trend in each country given the number of results returned. 

The results that returned for the staple pieces are the following. Jeans were most popular in France with over 12000 search results. While in comparison the US had the least amount of search results of all countries. T Shirts  were most popular in spain while least popular in the US. Sneakers were most popular in spain and least popular in the US. Sweaters were most popular Germany and lease popular in Spain. 

The results for fast fashion were the following. Cargo was overall very popular in all countries but seemed to be the most popular in France and Italy. Once again the US had the least amount of search results for a style of clothing. Leather was popular in spain and least popular in Germany. Overalls were very popular in Italy while not as popular in the US. Animal Print was most popular in Australia but not popular in Germany. 

Ultimatly, if a fashion manufacture is trying to make money they might want to consider where they market their product. For example, a company producing overalls might want to enter the italian market as there is a higher search result for overalls in Italy than in the United States. Though these example are meant to be takin with a grain of salt. This becomes increasing apparent when discussing the limitations of the ASOS API. The first limitation is language. When changing the country in the api the language was also changed. Thus, it was up to us to decide what was the most appropriate translation of a style. The consequence of which meant that meaning might be removed or added to the translated word. In other words, Italy might have more search results for overalls because in italian the translated word for overalls might encompass more than the English definition of overalls. Location was the second limitation of the API. European countries have access to three warehouse while the US only has one. Therefore, countries in europe might have more inventory to choose from than the US by default. This may explain why the US was most often the country with the least amount of search results returned for a style. 


### Abishai Conclusion:

The initial assumption we had was that women shop more across all countries. The function we enabled with the API allowed for search term, associated country, and corresponding country store. We were able to output horizontal bar graphs that displayed information of items and sum of its search results. Across countries of the US, AU (Australia), IT (Italy), DU (Germany), FR (France). Most of the graphs depicted higher search results for women. Factors that may contribute to the outputs include the API being in real time and current season. 

In order to flesh out inference supported by search results outputted from the APOS API, we collected data from the csv dataset. The Myntra CSV provided data from India’s e-commerce of product brand/ID, whether it is bought by each gender, number of images per item, item’s primary color, price (in indian rupees), and item description. 

From this dataset, we were able to narrow down the eight most popular brands and determine its popularity between each gender which provided insight into their spending habits. These top brands were determined by how often they appeared in the dataset. These top eight brands were Roadster, Park Avenue, Flying Machine, Puma, GORDANO, Mast & Harbour, and HERE&NOW. The first four brands were purchased a lot more by men. The last three brands didn’t have as big of a difference between them however, women purchased more of those brands respectively. In conclusion, according to the myntra csv dataset, we can say that men shop more than women. 
