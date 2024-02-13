# BasketballProject

Were NBA players more valuable in the 80's-00's than today?

Win Shares is the metric I analyzed to measure player value.

Here is the Win Shares definition: 
Win Shares is a player statistic that attempts to divvy up credit for team success to the individuals on the team.

You can click this link if you want to learn more about how win shares are calculated. 
https://www.basketball-reference.com/about/ws.html

To start my analysis, I pulled up the top 250 single-season win share totals (see link). 
https://www.basketball-reference.com/leaders/ws_season.html

To start digging into the data, here was the information that I needed:
1. The player's name.
2. The season in which the win share total occurred.
3. The position the player played.
4. The amount of win shares the player accounted for.

I pulled the data by web scraping via BeautifulSoup and Selenium Webdriver. See WSCode

Since I wanted to analyze the BEST of the BEST, I narrowed my sample from 250 to 96. The number is 96 because I wanted to do the top 100 seasons, but some of the rows I scraped did not have player data. As a result, the final count ended up being 96. 

Once I decided on the final number, I created a DataFrame and added my four data points (player name, season, position, winshares).

To answer the question above (Were NBA players more valuable in the 80's-00's than today?), I needed to group the top 96 win share seasons by decade. 

I looped through my Win Shares dataFrame and ran if statements based on the third digit in the year (19**7**0). For this analysis 1979-1980 would be considered the 70's and 1989-1990 would be considered the 80 (see DecadeLoops).

**Here are the results:**

![Top96PieChart](https://github.com/clarkeallan931/BasketballProject/blob/main/WSPieChart.png)

**Data that stood out:**

- There were zero players in the 2020s that made it into the top 96 win-share total. (Nikola Jokic was 99th in 2020-2021)
- The amount of high-level win share season started declining drastically after 2010.
- The '60s and '70s were the decades with the highest percentage of top Win Share seasons. 

Are players less valuable today? Or a there other factors at play? 

When examining the Win Share definition, I noticed that it is not calculated on a per-minute basis. That means star players (players who play more) will have a higher Win Share total even if they are less productive/efficient on a per-minute basis. 

Is it possible that players played more minutes in the 60's-00's than they do today? 

Now I want to find the "star" players average minutes per game in 2001 and 2024. The reason why I picked 2001 it was in a decade that had similar-level athletes 

To conduct this analysis I needed to find the minutes per game for the top 25 scorers in each of those years. 

I created to summary stats table to see how the production and playing time have changed since 2001.

**Here are the results**









