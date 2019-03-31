Being a Bayern Munich supporter injuries have been a big part of past campaigns I have followed. During most of the past season (2017/2018) Manuel Neuer was injured with a broken foot. For the second match against Real Madrid in the Champions League semi finals the team had to additionally compensate the injuries of Jerome Boateng, Arturo Vidal, Kingsley Coman and Arjen Robben. While Pep Guardiola was still coach at Bayern his dispute with the long-serving team doctor Mueller-Wohlfahrt culminated into him resigning after 38 years with the team (Mueller-Wohlfahrt was later reinstated as the team doctor in 2017).

The Data
--------

There is not much structured and comparable data out there on injuries and time lost due to injuries (at least not that I am aware of). The great website [fussballverletzungen.com](http://fussballverletzungen.com/) (on German) regularly surveys type, duration and frequency of all injuries across the Bundesliga. Transfermarkt has a pretty detailed overview of missed matches for each player, but it makes it hard to compare the impact across teams. We need to aggregate this data for each team and normalize it.

### A few things we should aim to adjust for to make the comparison meaningful:

-   Squad size varies considerably across teams. To show two extremes: Borussia Dortmund starts the current season with 29 players, Bayern Munich with 23. Simply comparing the absolute number of players injured will therefore distort the picture
-   The Transfermarkt data frequently includes youth players in the squad. An injury of such a player would be less severe for a team compared to a regular first-team player.

To mitigate the above problems I will weigh each player by their relative contribution to the team's market value. We will therefore both adjust for the squad sizes and for the relative importance of each player. One downside is that we will naturally overweight younger players compared to older players. Another option may be to weigh by player strength (e.g. FIFA rating) but I currently don't have these readily available.

For a start, I will below show a time series of *% of players injured (weighted by market value)* for some of the top European clubs. The data is for their domestic league and covers the past five completed seasons: 2013/2014 to 2017/2018.

To introduce some kind of relative benchmark I computed the average of the above statistics for the covered clubs across all seasons: on average 14.8% of players are injured at any given time.

Find below the plots split by league starting with the Bundesliga starring Bayern Munich and Borussia Dortmund.

### Bundesliga

![](bundesliga.png)

Both Bayern and Dortmund have a problem with a high injury rate across their players. They consistently have a larger-than-average percentage of their squad injured. This is even more surprising as the Bundesliga has both fewer games each season than the other four leagues, and also the longest break around New Year which should be beneficial for regeneration. The Bundesliga is also one of the less competitive leagues which should give at least Bayern plenty of opportunity to rest key players.

### Premier League

![](premier_league.png)

Over the first three seasons covered Arsenal showed high injury rates but has greatly improved them since 2016. It will be interesting to observe if this continues or if this is just a blip caused by them only playing the Europa League last season. We see a similar but not as extreme pattern for Manchester City.

### La Liga

![](la_liga.png)

All three Spanish teams show low injury rates. Especially Atletico and Barcelona show consistently low rates. Given all three teams play in a very competitive league and usually have the additional burden of Champions League matches this is astonishing. FYI, the two sudden spikes we observe for Barcelona are caused by short-term injuries of Messi.

### Serie A

![](serie_a.png)

Not much to say about Juventus. They seem to be able to keep injury rates pretty low and constant.

### Ligue 1

![](ligue_1.png)

For PSG we uncover some of the extremes driven by our methodology. For the majority of the analyzed period PSG shows a below-average injury rate. However the injury of Neymar at then end of the 2017/2018 season heavily distorts the picture. With an estimated transfer value of €180m Euros he makes up roughly 20% of PSG's team value alone.

### Next Steps

There are a bunch of questions you can tackle with this kind of data. Are there any teams which are just better at preventing injuries? Does the data change if we split injuries into *preventable* (muscle injuries) and *non-preventable* (illnesses and broken bones)? Are players with a history of severe injuries more injury-prone going forward? Is there a correlation between workload/matches played and injury rates?