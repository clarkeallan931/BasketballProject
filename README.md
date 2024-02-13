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

I looped through my winshares dataFrame and ran if statements based on the third digit in the year. 19**7**0





