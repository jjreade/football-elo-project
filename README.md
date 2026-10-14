# football-elo-project

Elo ratings, as devised by Arpad Elo, are a very simple way of tracking how good participants in sporting contests are. They underpin many official rankings in different sports. In football, for national teams [eloratings.net](https://eloratings.net/) provides Elo ratings, while [clubelo.com](https://www.clubelo.com/) does the same for club teams.

I have long calculated Elo ratings for my own research purposes, slightly tweaking the method as I've gone along, without ever making the ratings or the method available. On this repo I'll aim to do that.

My ratings were used in the State of the Game Report released by the Independent Football Regulator in England, in part because of coverage. I use results data I've scraped from Soccerbase, alongside other sources to go back to 1866. This means that my ratings both cover a very long period of time (and I hope that this historic coverage will continue to expand), and a lot of teams - down below the Football League in England, and they cover all the competitions that Soccerbase has expanded to in recent years.

The ratings are collected as follows:
- Pre 1890 football matches (in England) can be found, with Elo ratings for each team and a prediction, [here](elo-pre1890s.csv).
- Matches in the 1890s can be found [here](elo-1890s.csv).

Please feel free to use these Elo ratings in your work, should they prove useful. If you do, please cite the following:
"Developing Elo Ratings for Club Football Matches”, Reade, J.J., De Angelis, L., and Singleton, C., 2026, Discussion Paper, Department of Economics, University of Reading.
