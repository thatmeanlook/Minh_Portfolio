# Minh Luc 
I'm a Data Science student at UC San Diego. Welcome to my page!


## “BOND, JAMES BOND.”

James Bond (007) is a British Secret Service agent created in 1953 by Ian Fleming. Over the years, there have been more than 20 movies with different famous actors portrayed the British agent. As a fan of the series, I want to look at the data to explore some interesting ideas. 

### Description of James Bond Dataset

I am going to work on the “James Bond Movie Dataset” from [Kaggle](https://www.kaggle.com/dreb87/jamesbond). This dataset includes information about 24 James Bond movies from 1962 to 2015.
![](https://github.com/thatmeanlook/Minh_Portfolio/blob/main/images/df.png)

  
Looking at the data, I want to explore these ideas:
  
* What do audience think about James Bond movies?

* Which Bond movie is the most successful?

* Who is the best rated Bond? 
  
### Data Cleaning
There are 27 columns in the dataset. Let’s cleanup and select the columns that are related to our exploratory
data analysis.

![](https://github.com/thatmeanlook/Minh_Portfolio/blob/main/images/bond_df2.png)

•	Year:  Release year of the movie 

•	Movie: The movie title

•	Bond: Actor who played James Bond

•	World_Adj: The film’s worldwide gross earning adjusted based on 2013

•	Budget_Adj: The film’s budget adjusted based on 2013

•	Avg_User_IMDB: The average user rating from IMDB

•	Avg_User_Rtn_Tom: The average user rating from Rotten Tomatoes

•	Shooting_Loc: Shooting locations of the movie

### Audience Acceptance

The first thing I want to do with this dataset is to see what the audience thinks of Bond movies over the years. Since the first release in 1962 to 2015, how has the rating changed? The dataset provides rating of each movie from IMDB and Rotten Tomatoes. Combine these 2 metrics, I can find the average rating of each movie. 
![](https://github.com/thatmeanlook/Minh_Portfolio/blob/main/images/rating_data.png)
 
Plotting a line graph to see the trend of rating over the year:

 
Looking at the graph, the series has a good start in the 60s with consistent rating over 7.5. However, it trends down in next 2 decades. The 80s witnesses the downfall of Bond, with rating dips below 5.5 at the lowest. Things start to look up for Bond since 2000s.
The rating for the series fluctuates over the years. One of the main contributing factors is who plays Bond, which bring us to the next point in this analysis.
Who is the best Bond?
There have been 6 changes of actor.  To get an average score for each actor, I take all the movies with the same actor and calculate the mean rating.
Fig.2 Each actor’s score 
With his class and charisma, there is no surprise that Sean Connery is rated the best Bond. Even though Daniel Craig is in second place, his rating is so close to Connery that the two can be considered as tie. Interestingly, Connery is the first actor to play Bond (1962) and Craig is the lasted one starting from 2006. 
Commercial Success
The James Bond series has been a familiar name at the worldwide box office. By looking the gross earning of all the movie, we can easily see which movie has the highest revenue. However, just looking at the revenue doesn’t give us the full picture. I’m also curious about the return on investment of each movie, in other word, the ratio between Budget and Revenue. 
 
2012’s “Skyfall” with Daniel Craig is the most commercially successful Bond film of all time, with over $1.1 billion at the worldwide box office. At second place is 1965’s “Thunderball” with Sean Connery. 
Looking at the Budget/Revenue ratio metric, “Dr.No” is unbeatable with a ratio of almost 60. This is an incredible return on investment. Second place on this list is 1964’s “Goldfinger.” 
 
Locations
As a secret agent with a mission to save the world, Bond has been to many exotic destinations, from snowy mountains in Switzerland to deserts in Chile. Using the Shooting location provided in the dataset, I calculated the frequency each country appears in the series. I then plotted a choropleth map to visualize where Bond has been:

 
Looking at the distribution on the map, England is on top of the list with 20 appearances over 24 movies. No surprise there since this is where Bond calls home. US, France and Italy are among the top locations chosen for Bond movies. Switzerland and Spain also appear in a few movies. It’ll be interesting to see where Bond’s next mission will take him.
