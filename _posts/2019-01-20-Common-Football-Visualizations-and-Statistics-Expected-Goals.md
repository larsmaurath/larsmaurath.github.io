More detailed and readily available data and a thriving analytics community on Twitter have produced a series of new statistics and visualizations for football fans. In this series I will try to give a brief definition of various metrics, background information on charts and sources for where to find them going forward.

Expected Goals
==============

The concept of *Expected goals* tries to quantify the quality of chances. To every shot it assigns a value between 0 and 1 based on the historical success rate (i.e. probability of scoring) of similar shots. Different properties of the shot can be used to assess its value: - Location on the pitch - Was the shot a header or a shot? - Did the shot occur during open-play or after a free kick/corner? - Did the shot follow a long series of passes or a rebound?

Advanced models also include defensive pressure, i.e. how defenders are positioned around the shot taker.

This metric can be useful in various ways: by comparing expected goals and actual goals for a single player we can assess how good his finishing is. Is his actual goal tally driven by his exceptional finishing or is his team generating countless chances for him and he could have scored even more?

For a single game we can compare xG values for both teams to get a sense if the final score was deserved. Team A may have created a large number of chances but was unlucky (or unskilled) in finishing. Team B may have won 1-0 by scoring a very low xG goal (think of a deflected long-range shot) while they created no other chances. Over a longer time period expected goals and actual goals of a team should converge; this allows us to judge if a team is currently actually very good or only lucky and bound to converge to its mean.

The concept of expected goals can also help coaches and players to make better decisions. Should players reduce the number of long-range shots they take? Should they instead make every effort to pass the ball into central positions close to goal? While the focus of xG debates are usually on attack, every aspect can also be applied to a team's defense.

The xG metric went mainstream when the BBC included it in its 'Match of the Day' program in the 2017/18 Premier League season. They now usually show the xG values for each team following the match summary.

xG Shot Maps
------------

Below chart of Harry Kane's World Cup shots shows one way to visualize xG for a single player. Each shot's location, type (shape of the marker), outcome (border of the marker) and xG value (color shading) are highlighted. Even in this very small sample we can already see that location both vertically (close to goal) and horizontally (ideally in the center of the goalmouth) plays an important part in determining the xG value. Charts similar to this are posted by different accounts. The one below was posted by [Statsbomb](https://statsbomb.com) a football data provider and consultancy. They collect their own data and even have some free data available on their website. They also have their very own [podcast](https://statsbomb.com/category/podcast/) which is a great source of background information on their work and football in general.

xG Flow Charts
--------------

xG flow charts visualize the development of xG values over the duration of a single match. Next to a simple comparison of final score to final xG values it also allows us to see the timing and quality of chances for each team. This can give us a sense of how the match unfolded and which team was dominant during which period. In the below chart we can see for example that Crystal Palace scored with very much their first chance while Liverpool racked up quite a few shots already without converting any. The chart also immediately tells us that while Firmino's 2:1 was a very low xG shot (on average this shot hardly ever converts to a goal), Salah's 3:2 was a very easy goal.

You can find these type of charts by following [BetweenThePosts](https://twitter.com/BetweenThePosts) on Twitter. This account runs a bot which posts this chart for most matches of the big-5 leagues.
