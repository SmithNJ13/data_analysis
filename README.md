# This repository contains the dataset I used in my analysis as well as the Jupyter Notebook I used to write up my python code:
``` analysis.ipynb ```

## The questions I examine in my analysis are the following:

**1.** Which team has scored the most goals in the past decade?
```
Man City, Total Goals: 956
```

**2.** Which team(s) in the past decade, win most of their games at home and which team(s) win most of their games away?
```
Interestingly, the team with the highest home win rate % is Middlesbrough with 80.0% of 
their wins at home. Ipswich have the highest away win rate % at 67.0%.
Ironically, despite these impressive values, both teams have their overall win rate % at 13.0%. Yikes.

In a more fair manner, if I want to make a meaningful observation, I decided to limit the pool to teams 
who have 50 or more wins. In this instance, Everton, with a total of 135 wins has a 
Home Win Rate% of: 64%! Meanwhile, Crystal Palace, with a total of 125 wins 
has an Away Win Rate% of: 47%!

Despite this, Everton has an overall Win Rate% of: 34.0%
and Crystal Palace has an overall Win Rate% of: 31.0%

On average, for teams with 50 or more wins, the mean Home Win Rate% was: 58% and,
the mean Away Win Rate% was: 42%.

What I can conclude from this is that:
 A. Home advantage is a *very real* thing. You are more likely to win at Home.

 B. Everton get most of their wins from playing at Home, coupled with their overall Win Rate% they are 
       not a particularly strong team. The few wins they do get, 
       the majority are because of Home advantage.

 C. Crystal Palace has a higher than average Away Win Rate% than other teams. This has no
       reflection on the teams ability. Teams like Man City who have a similar value
       (46% Away Win Rate) have a significantly better performance and higher overall Win Rate%.

 D. In summary, looking at Home Win Rate% and Away Win Rate% has no real significant impact 
       in determining a teams ability, or their performance. Other than identifying that 
       Home advantage is a thing that affects all teams.

 E. To further analyse this, I looked at teams overall Win Rate% in relation to their Home Win Rate% 
       and Away Win Rate%. 
       HomeWinRate >= 58, Avg overall Win Rate%: 37%, HomeWinRate < 58, Avg overall Win Rate%: 43%
       AwayWinRate >= 42, Avg overall Win Rate%: 43%, HomeWinRate < 42, Avg overall Win Rate%: 37%

       Teams that rely mostly on Home Wins on average have worse overall Win Rate%, and teams
       with higher Away Win Rate% on average have better overall Win Rate%.
       To conclude, teams must excel both at Home and Away to be considered a strong team.
```


**3.** Is there a correlation between the number of shots taken by a team and the number of goals they score?  

**4.** Has fouling become more frequent over the years and what can one conclude from the findings?  

**5.** What factors impact a team's ability to win the most?  
