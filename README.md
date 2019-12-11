# Matt_Mod02_Project

## Author: Matthew_Newton

### Introduction

### Database structure

The SQL data base information is drawn form https://www.kaggle.com/laudanum/footballdelphi

#### Four Tables in Database:
###### Matches:	            
24625 x 9
Match_ID, Div, Season, Date, HomeTeam, AwayTeam, FTHG, FTAG, FTR

###### Teams:	              
468	x 8
Season, TeamName, KaderHome, AvgAgeHome, ForeignPlayersHome, OverallMarketValueHome, AvgMarketValueHome,StadiumCapacity

###### Teams_in_Matches:
49148 x 2
Match_ID, Unique_Team_ID

###### Unique_Teams:
128 x 2
TeamName, Unique_Team_ID


#### Matches
Match_ID (int): unique ID per match
Div (str): identifies the division the match was played in (D1 = Bundesliga, D2 = Bundesliga 2, E0 = English Premier League)
Season (int): Season the match took place in (usually covering the period of August till May of the following year)
Date (str): Date of the match
HomeTeam (str): Name of the home team
AwayTeam (str): Name of the away team
FTHG (int) (Full Time Home Goals): Number of goals scored by the home team
FTAG (int) (Full Time Away Goals): Number of goals scored by the away team
FTR (str) (Full Time Result): 3-way result of the match (H = Home Win, D = Draw, A = Away Win)

#### Teams
Season (str): Football season for which the data is valid
TeamName (str): Name of the team the data concerns
KaderHome (str): Number of Players in the squad
AvgAgeHome (str): Average age of players
ForeignPlayersHome (str): Number of foreign players (non-German, non-English respectively) playing for the team
OverallMarketValueHome (str): Overall market value of the team pre-season in EUR (based on data from transfermarkt.de)
AvgMarketValueHome (str): Average market value (per player) of the team pre-season in EUR (based on data from transfermarkt.de)
StadiumCapacity (str): Maximum stadium capacity of the team's home stadium

#### Unique Teams
TeamName (str): Name of a team
Unique_Team_ID (int): Unique identifier for each team

#### Teams_in_Matches
Match_ID (int): Unique match ID
Unique_Team_ID (int): Unique team ID (This table is used to easily retrieve each match a given team has played in)

### Summary Methodology

### Summary Findings

### Conclusion
