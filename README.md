## Data Science Project 2 - Soccer Win Rate Hypotheses
**Created by:** Andy Luc and Taeho Jeon  
**Student Pace:** Full-Time Data Science  
**Scheduled project review date/time:** 05/10/2019  
**Instructors:** Miles Erickson & Greg Damico  
**Slide Deck Presentation:** 

Our company name is Datakick Inc., and we provide performance stats for over 250 European League soccer teams to other companies on whether or not certain factors can contribute to a win or loss. Our hypothesis analyses will also provide a good indicator on future predictions regarding league performance and increased accuracy on betting odds.

### Focused Questions:  
Is there a statistical difference in the odds of...
1. Winning a game when a team is playing in front of their home crowd?
2. Winning a game when the players’ height of the home team is taller?
3. Losing a game when the defensive pressure of a team is lower than the other team?
4. Winning a game when a team has higher offensive attributes(passing & shooting) than the other team?
5. Winning a game when a team is playing in front of their home crowd vs away crowd?

### Data Set:   
The data was obtained from a large SQlite file found on kaggle(https://www.kaggle.com/hugomathien/soccer). We had then extracted each table in the SQlite file into 7 different .csv files, and imported them into a newly created database called “football_db” in PostgreSQL. This included: Country, League, Match, Player, Player Attributes, Team, and Team Attributes.

### Hypothesis Process: 
Through sample T-testing, null and alternative hypotheses were written to support our critical questions. Using the new *football_db* database in PostgreSQL, several queries were made to form relevant dataframes for our calculations. For each hypothesis, a sample size for the number of games was set against our variable. Next, we calculated the mean and standard deviation, and compared the variances. A t-stat was ultimately generated, which gave us a p-value to measure our data. With of an alpha at 5% (where we either accept or reject a null hypothesis), our results are as follows:
- There is *no* statistical difference when a team wins in front of a home crowd
- There is *no* statistical difference when a team wins based on the height of teams players
- There *is* a statistical difference when a team loses based on the teams' defense pressure
- There is *no* statistical difference when a team wins based on the teams' offensive attributes(passing & shooting)
- There *is* a statistical difference when a team wins in front of a home crowd vs away crowd
