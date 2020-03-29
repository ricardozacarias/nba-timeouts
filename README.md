# Calling timeouts in the NBA

###### by Ricardo Zacarias

*For fully interactive version of this story go [here](https://ricardozsilva.wixsite.com/take-that-for-data).*



As I get up to snack after watching another delicious fried chicken ad, I started wondering about how much of my life was being wasted by timeouts in NBA games. 

> *In the National Basketball Association (NBA), teams are allowed seven timeouts, each of 1 minute, 15 seconds. There is no limit on substitutions. In overtime periods, each team is allowed two timeouts. A timeout can only be requested by a player in the game or the head coach, and only when the ball is dead or in control of the team making the request.*

I wanted to get an accurate number of how many are used during a season, but I quickly discovered that timeout stats are not very common in game box scores. Still curious, I found some play-by-play data available [here](https://eightthirtyfour.com/data) and decided to have a go at it myself.

I found **13,437** total timeouts during the 2018-19 regular season. 

**6,652** taken by the home team, and **6,785** by the visiting team.

Below you can see on hover how much time your favorite team has cost you in timeouts (if you watched all 82 games, of course).

<div>
    <a href="https://plotly.com/~Zaca/45/?share_key=TsTShGlZ4ozuXYbdpmGr5v" target="_blank" title="TimeoutsPerTeam3" style="display: block; text-align: center;"><img src="https://plotly.com/~Zaca/45.png?share_key=TsTShGlZ4ozuXYbdpmGr5v" alt="TimeoutsPerTeam3" style="max-width: 100%;width: 850px;"  width="850" onerror="this.onerror=null;this.src='https://plotly.com/404.png';" /></a>
    <script data-plotly="Zaca:45" sharekey-plotly="TsTShGlZ4ozuXYbdpmGr5v" src="https://plotly.com/embed.js" async></script>
</div>

The first thing I noticed was that teams displayed more variability in the use of timeouts than I had anticipated. Rockets fans profit most from Mike D'Antoni's notorious reluctance in stopping the game:

> "What am I gonna do, say 'Oh, let me take the ball out of James's hand, then take it out, call a timeout, put it back in their hands in the exact same spot they were?' We just go with it." D'Antoni said in an [interview](https://www.si.com/nba/2019/05/02/steve-kerr-gregg-popovich-mike-dantoni-brad-stevens-brett-brown-nba-coaches-playoffs-timeouts) with Sports Illustrated earlier this year. 

Interestingly, he used to be the assistant to 76ers coach Brett Brown who sits on the other end of the spectrum. In the same interview he mentions that he never challenged his previous boss about all the voluntary stoppages. "The biggest thing, I thought," he said, "was that it ate into my dinner time." I feel you Mike.

We all know the very end of close games can be quite painful thanks to TO calls, but I wondered how they are used during the rest of the game.

<div>
    <a href="https://plotly.com/~Zaca/41/?share_key=uYvfNc087aOYW8J7w1Ue6l" target="_blank" title="TimeoutsOverTime2" style="display: block; text-align: center;"><img src="https://plotly.com/~Zaca/41.png?share_key=uYvfNc087aOYW8J7w1Ue6l" alt="TimeoutsOverTime2" style="max-width: 100%;width: 800px;"  width="800" onerror="this.onerror=null;this.src='https://plotly.com/404.png';" /></a>
    <script data-plotly="Zaca:41" sharekey-plotly="uYvfNc087aOYW8J7w1Ue6l" src="https://plotly.com/embed.js" async></script>
</div>
The pattern of timeout calling is similar for the first three quarters, but as we all know, everything changes in the fourth. You'll notice that both peaks occur at the same time in the first 3 periods, when there's 6:45 and 2:45 left in the quarter. I had no idea about this, but these times match mandatory TV timeouts defined by the league. From the official NBA rulebook:

> *"There must be two mandatory timeouts in each period.* *If neither team has taken a timeout prior to 6:59 of the period, it shall be mandatory for the Official Scorer to take it at the first dead ball and charge it to the **home team**. If no subsequent timeouts are taken prior to 2:59, it shall be mandatory for the Official Scorer to take it and charge it **to the team not previously charged**."*

If this is true then the first peak in each quarter should be dominated by the home team calling timeout and the second peak by the visiting team. I separated the blue trace by the team making the call (red - home, orange - away) and you can click on the legend line to activate or deactivate traces.

The 4th quarter is a special case. There are still two peaks, but quite different from the others. The first real bump occurs at 3:15, **before** the 2:59 threshold for a TV break meaning these are not mandatory timeouts. If you keep reading the rule book:

> *"Each team will be limited to two team timeouts after the three-minute mark of the fourth period".*

The high frequency of TOs at this time is most likely caused by coaches not wanting to waste them by going into the end of the game with more than 2 left. And naturally, the very end of the game is timeout galore.

This suggests that not all timeouts are the same. Next, I wondered about the current state of the match when coaches decide to intervene, so I looked at the distribution of score differentials at timeout events. 

