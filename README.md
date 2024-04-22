# Cricket-Data-Analytics-Project

**Aim** : To filter out batsman and bowlers from the T20 Men's World Cup and see which players performed exceptionally well.

**Soruce of the data** : ESPNCricInfo (https://www.espncricinfo.com/records/tournament/team-match-results/icc-men-s-t20-world-cup-2022-23-14450)

**Parameters Scoping**:

**Batsman:**
1. **Strike rate** (No of runs scored per 100 balls) > 140
2. **Batting Average** (Average runs scored in an innings ) > 30
3. **Innings batted** (Total Innings batted) > 3
4. **Boundary %** (% of runs scored in boundaries)  > 50

**Bowler:**
1. **Strike rate** (Average no. of balls required to take a wicket) < 16
2. **Average** (No. of runs allowed per wicket) < 18
3. **Innings bowled** (Total Innings bowled) > 4
4. **Dot ball %** (% of dot balls bowled) > 40


**Tasks Performed** : 
1. Performed **Web Scraping** using 2 techniques:
     a) Using Python Library **Beautiful Soup**
     b) Using an online web data collector, **Bright Data** which required javascript to scrape the data and then converted it into downloadable json files
2. Used json files to perform **Exploratory Data Analysis** and then converted and stored files in CSV format.
3. Transformed data and values using **DAX model** in Power BI 
4. Developed interactive report using **Power BI** 
