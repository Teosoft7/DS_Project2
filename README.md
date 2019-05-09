## Data Science Project 2 - Soccer Win Rate Hypotheses
**Created by:** Andy Luc and Taeho Jeon 
**Student Pace:** Full-Time Data Science  
**Scheduled project review date/time:** 05/10/2019  
**Instructors:** Miles Erickson & Greg Damico  
**Slide Deck Presentation Link:** 

Our company name is datakick.inc, and we provide performance stats for over 250 soccer teams to other companies on whether or not they can contribute to a win or loss. Our data will also provide a good indicator on future predictions regarding league performance and betting odds.

**Focused Questions:**
  1. Is there a statistical difference in the odds of winning a game when a team is playing in front of their home crowd?
  2. Is there a statistical difference in the odds of winning a game when the height of a team is taller than the other team?
  3. Is there a statistical difference in the odds of losing a game when the defense pressure of a team is higher than the other team?

**Hypotheses Process** 
Through 1-sample and 2-sample testing, we formed a null and alternative hypothesis to answer our focused questions. Initially, we converted our sqlite dataset into postgresql, and then converted each table into .csv files (Country, League, Match, Player, Player Attributes, Team, Team Attributes). Next, we pulled our relevant values in SQL and created a dataframe for each of the tables in our code. With detailed hypothesis testing, inclusive of an alpha at 5% (where we either accept or reject a null hypothesis), our results are as follows:

- There *is no* statistical difference when a team wins in front of a home crowd or wins at away games
- There *is no* statistical difference when a team wins based on the height of teams players
- There *is* a statistical difference when a team loses based on the teams' defense pressure
