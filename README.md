# This repository contains the dataset I used in my analysis as well as the Jupyter Notebook I used to write up my python code:
``` analysis.ipynb ```

## The questions I examine in my analysis are the following:

**1.** Which team has scored the most goals in the past decade?
```
1st Man City, Total Goals: 989

    2nd: Liverpool, Total Goals: 876

        3rd: Arsenal, Total Goals: 777
```

**2.** Which team(s) in the past decade, win most of their games at home and which team(s) win most of their 
games away?
```
Interestingly, the team with the highest home win rate % is Middlesbrough with 80.0% of 
their wins at home. Ipswich have the highest away win rate % at 67.0%.
Ironically, despite these impressive values, both teams have their overall win rate % at 13.0%. Yikes.

In a more fair manner, if I want to make a meaningful observation, I decided to limit the pool to teams 
who have 50 or more wins. In this instance, Everton, with a total of 135 wins has a 
Home Win Rate% of: 64%! Meanwhile in joint first, we have:
Chelsea, with a total of 210 wins and Crystal Palace, with a total of 125 wins,
both teams with an Away Win Rate% of 47.0%!

Despite this, Everton has an overall Win Rate% of: 34.0%
and Crystal Palace has an overall Win Rate% of: 31.0%

On average, for teams with 50 or more wins, the mean Home Win Rate% was: 58% and,
the mean Away Win Rate% was: 42%.

What I can conclude from this is that:
 A. Home advantage is a *very real* thing. You are more likely to win at Home.

 B. Everton get most of their wins from playing at Home, coupled with their overall Win Rate% they are 
       not a particularly strong team. The few wins they do get, 
       the majority are because of Home advantage.

 C. Crystal Palace & Chelsea have a higher than average Away Win Rate% than other teams. This has no
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


**3.** Is there a correlation between the number of shots taken by a team and the number of goals they score,
additionally, what deeper findings can you extrapolate from these statistics?
```
There is a strong correlation between shots taken and goals scored, with a slightly weaker - but still
strong correlation between shots on target and goals scored.

In addition to this I created three new novel metrics to assist with my analysis, these were the following:
1.    TSCR% (Total Shot Conversion Rate): Goals per total shots taken
2.    OTCR% (On Target Conversion Rate): Goals per shots on target
3.    ASC (Average Shot Coefficient): Team's shot frequency compared to season mean

Teams with high OTCR% achieved significantly better win rates (~61.6%)
Poor finishing teams, low OTCR%, struggled to win (~18.4% win rate)
Higher shot volumes correlate more strongly with goals than shot accuracy alone

Manchester City: High-volume shooting strategy with good conversion rates
Liverpool: Similar high-volume approach but lower conversion efficiency
Arsenal/Chelsea: More balanced approach between shot volume and accuracy

Man City had a very consistent ASC rating, averaging +0.91 across the entire decade! Meaning that
of all the Premier League teams active throughout that time, Man City were often the team
taking the most shots in a game - this can be indicative of a teams attacking tempo.

From these statistics that I worked with, there was a strong indication that Man City
over the last decade has been one of the most consistent and high performing teams in the League.
Conversely, of the EPL teams that have played every season since 2014, Crystal Palace on the whole
tends to be one of the most - arguably the most, underperforming team. There is a case to be made
against West Ham too, however, statistically their peaks were much higher, whereas
Crystal Palace never had amazing peaks, both in WinRate% or attacking tempo.

Of all 35 teams that have played in the EPL across the last decade (2014-2024),
Middlesbrough was categorically the worst, performing terrible in every meaningful metric and
often being the last, or second to last in the list. The following metrics are:

13.2% WinRate, 41.8% Shots on Target (Which, I have evaluated and shown has a negative 
correlation on performance),

18.5% OTCR% (On Target Conversion Rate), 7.7% TSCR% (Total Shot Conversion Rate) 

and a whopping -0.94 ASC (Average Shot Coefficient)

This means that Middlesbrough, had many of their shots on target, but the vast majority of them did 
not convertto goals - indictating a poor finishing performance. A terrible, TSCR% rate means that the 
shots they were takingthat are not on target are of rather poor quality and poor shot selection, 
and in addition to this, they weren'teven shooting that often. In the one season they played, they were 
close to being the bottom in total shots made. So of the very very few shots they decided to take, 
they were poor choices and they had no finishing.
This is reflected in their astronomically low Win Rate of 13.2%.

So if anyone asks you who the worst Premier League team of the last decade has been 
- Middlesbrough wouldn't be a terrible answer to give.
```

