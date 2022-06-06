# TMDB-Movie-Analysis
We answer the question - what steps can a production movie take to make a profitable movie?
## Questions posed:
 a The most profitable movie genre year by year
 
 b Top 10 Most profitable movies and least profitable movies
 
 c Properties associated with high revenue movies
 d Top 20 Highest-grossing Actors

## How each question was answered:
 a) The most profitable movie genre per year:
 
     -  Split the genre column and made each split genre a separate row
     
     -  Grouped the dataset by year and found the highest genre by popularity for that year
     
     -  Used a scatterplot to visualize the popularity of genres across several years (1960-2015)

 b) Top 10 Most profitable movies and least profitable movies
 
     - Created two datasets called dfTop10 and dfBottom10 respectively from the original movie dataset of just two columns (“original_title”,”net_profit”). 
     
     - Sorted dfTop10 by net_profit in descending order and limited it to 10 rows. This gave the Top 10 most profitable movies 
     
     - Sorted dfBottom10 by net_profit in ascending order and limited it to 10 rows. This gave the Top 10 least profitable movies

 c)  Properties associated with high revenue movies:
 
    - Calculated the mean revenue of the entire dataset. Then filtered the dataset to movies whose revenue that are higher than the revenue mean. Called this new dataset "dfHighProfit".
    
    -  Found the columns of dfHighProfit which had the strongest correlation to revenue.
    
 d) Top 20 Highest-grossing Actors on average:
 
    - Split the cast column and made each split cast a separate row. This is done so that each row has a single actor.
    
    - Grouped the dataset by “cast” column and calculated the average revenue generated per actor. Saved the result as a dataset called df1cast.
    
    -  Grouped the dataset by “cast” column and calculated the number of movies per actor. Saved the result as a dataset called df1castsum
    
    -  Merged df1castsum into df1cast and limited the dataset to actors with at least 10 movies. 
    
    -  Sorted df1cast dataset by average revenue in descending order and limited the dataset to the first 20 rows. 
    
    -  Generated a horizontal bar plot to visualize the highest average revenue per movie for the actors in the top 20 rows.


