# Football_API's - Mod02_Project

### Introduction

This project's objectives is to show the ability to use of APIs for web-scraping and Databases, to answer basic question.

Database is an SQL file set on football matches in England and Germany. See Appendix for details.
API is the DarkSky API which can be found at https://darksky.net/dev

Questions:
* The name of the team
* The total number of goals scored by the team during the 2011 season
* The total number of wins the team earned during the 2011 season
* A histogram visualisation of the team's wins and losses for the 2011 season (store the visualisation directly by assigning it to a variable)
* The team's win percentage on days where it was raining during games in the 2011 season.

### Summary Methodology

For the first 4 questions;
* Extract the data required to answer the question from the SQL databases.
* Manipulate in Pandas
* Finalise a Pandas DataFrame
* Present information in appropriate graph

Questions 5:
* Find the dates of all matches in the 2011 season for the German teams.
* Create a function to request the weather in Berlin for those dates.
* Export that to a CSV for later use.
* Import the CSV and merge it to the matches dataframe obtain for the dates.
* Manipulate to give percentage of games won in the rain.

### Summary Findings
Question 1:
There are 128 unique teams in the dataset.

Question 2:
See df_2011 for the brake down.
Man_City had the best goal difference with +64.

Question 3:
See df_results_2011 for brake down:
Man_United & Man_City both had 28 wins for the season 2011.

Question 4:
See NewWorkbook

Question 5:
Karlsruhe had a 7:1:0 win:draw:loss ratio for the 2011 Season.

### Conclusion
All question answered although I had difficulty in producing graphs to display my answers.

I did not complete: The MongoDB data base or Storing Function in a separate Python File.

The most difficult thing was certainly the API data request & extraction to database.

I would like to give this another shot at some point.  

### Database Structure Appendix:

The SQL data base information is drawn form https://www.kaggle.com/laudanum/footballdelphi

#### Four Tables in SQL Original Database:

##### Matches:	            
24625 x 9

Match_ID, Div, Season, Date, HomeTeam, AwayTeam, FTHG, FTAG, FTR

##### Teams:	              
468	x 8

Season, TeamName, KaderHome, AvgAgeHome, ForeignPlayersHome, OverallMarketValueHome, AvgMarketValueHome,StadiumCapacity

##### Teams_in_Matches:
49148 x 2

Match_ID, Unique_Team_ID

##### Unique_Teams:
128 x 2

TeamName, Unique_Team_ID
