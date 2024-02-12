# BasketballProject

Were NBA players more valuable in the 80's-00's than they are today?

Win Shares is the metric I analyzed to measure player value.

Here is the Win Shares definition: 
Win Shares is a player statistic which attempts to divvy up credit for team success to the individuals on the team.

Click this link if you are interested in learning more about how win shares are calculated. 
https://www.basketball-reference.com/about/ws.html

To start my analysis, I pulled up the top 250 single season win share totals (see link). 
https://www.basketball-reference.com/leaders/ws_season.html

To start really digging into the data, here was the information that I needed:
1. The player name.
2. The season in which the win share total occured.
3. The position the player played.
4. The amount of win shares the player accounted for.

I pulled the data by webscraping via BeautifulSoup and Selenium Webdriver. See WS Webscraping Code

