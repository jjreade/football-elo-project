# football-elo-project

Elo ratings, as devised by [Arpad Elo in 1978](https://gwern.net/doc/statistics/order/comparison/1978-elo-theratingofchessplayerspastandpresent.pdf), are a relatively simple way of tracking how good participants in sporting contests are. They underpin many official rankings in different sports. They are equally calculated by many people due to the [method being readily available for coding](https://en.wikipedia.org/wiki/Elo_rating_system). In football, for national teams [eloratings.net](https://eloratings.net/) provides Elo ratings, while [clubelo.com](https://www.clubelo.com/) does the same for club teams.

I have long calculated Elo ratings for my own research purposes, slightly tweaking the method as I've gone along, without ever making the ratings or the method available. On this repo I'll aim to do that, based on a research collaboration with Carl Singleton and Luca De Angelis.

My ratings were used in the State of the Game Report released by the Independent Football Regulator in England, in part because of the leagues and teams the cover. I use results data I've scraped from Soccerbase, alongside other sources to go back to 1866. This means that my ratings both cover a very long period of time (and I hope that this historic coverage will continue to expand), and a lot of teams - down below the Football League in England, and they cover all the competitions that Soccerbase has expanded to in recent years.

The ratings are collected as follows:
- Pre 1890 football matches (in England) can be found, with Elo ratings for each team and a prediction, [here](data/elo-pre1890s.csv).
- Matches in the 1890s can be found [here](data/elo-1890s.csv).
- Matches in the 1900s can be found [here](data/elo-1900s.csv).
- Matches in the 1910s can be found [here](data/elo-1910s.csv).
- Matches in the 1920s can be found [here](data/elo-1920s.csv).
- Matches in the 1930s can be found [here](data/elo-1930s.csv).
- Matches in the 1940s can be found [here](data/elo-1940s.csv).
- Matches in the 1950s can be found [here](data/elo-1950s.csv).
- Matches in the 1960s can be found [here](data/elo-1960s.csv).
- Matches in the 1970s can be found [here](data/elo-1970s.csv).
- Matches in the 1980s can be found [here](data/elo-1980s.csv).
- Matches in the 1990s can be found [here](data/elo-1990s.csv).
- Matches in 2000 can be found [here](data/elo-2000.csv).
- Matches in 2001 can be found [here](data/elo-2001.csv).
- Matches in 2002 can be found [here](data/elo-2002.csv).
- Matches in 2003 can be found [here](data/elo-2003.csv).
- Matches in 2004 can be found [here](data/elo-2004.csv).
- Matches in 2005 can be found [here](data/elo-2005.csv).
- Matches in 2006 can be found [here](data/elo-2006.csv).
- Matches in 2007 can be found [here](data/elo-2007.csv).
- Matches in 2008 can be found [here](data/elo-2008.csv).
- Matches in 2009 can be found [here](data/elo-2009.csv).
- Matches in 2010 can be found [here](data/elo-2010.csv).
- Matches in 2011 can be found [here](data/elo-2011.csv).
- Matches in 2012 can be found [here](data/elo-2012.csv).
- Matches in 2013 can be found [here](data/elo-2013.csv).
- Matches in 2014 can be found [here](data/elo-2014.csv).
- Matches in 2015 can be found [here](data/elo-2015.csv).
- Matches in 2016 can be found [here](data/elo-2016.csv).
- Matches in 2017 can be found [here](data/elo-2017.csv).
- Matches in 2018 can be found [here](data/elo-2018.csv).
- Matches in 2019 can be found [here](data/elo-2019.csv).
- Matches in 2020 can be found [here](data/elo-2020.csv).
- Matches in 2021 can be found [here](data/elo-2021.csv).
- Matches in 2022 can be found [here](data/elo-2022.csv).
- Matches in 2023 can be found [here](data/elo-2023.csv).
- Matches in 2024 can be found [here](data/elo-2024.csv).
- Matches in 2025 can be found [here](data/elo-2025.csv).
- Matches in 2026 can be found [here](data/elo-2026.csv).

Each file is organised as follows:
- date: the date the match took place on
- team1: the team listed first (usually the home team)
- goals1: goals scored by the team listed first
- goals2: goals scored by the team listed second
- team2: the team listed second (usually the away team)
- Elo predictions (elopredict.[type], elostrength.[type].1, elostrength.[type].2):
  - elopredict.kovalchik.dbl: Exponential decay with each match of a club's existence and current season
  - elopredict.decay: A decay factor for if a team hasn't played in a long time.
  - elopredict.home.adv: Adding a home advantage parameter into the calculation.
  - elopredict.goal.diff: Using goal difference in matches to update Elo ratings.
  - elopredict.cup: Increasing the weight for cup matches.
  - elopredict.full: All of the above
  - elopredict.base1: K adjustment factor = 1
  - elopredict.base5: K adjustment factor = 5
  - elopredict.base10: K adjustment factor = 10
  - elopredict.base20: K adjustment factor = 20
  - elopredict.base40: K adjustment factor = 40
  - elopredict.clubelo: Elo predictions from clubelo (via [xgabora's Github](https://github.com/xgabora/Club-Football-Match-Data).

I will update these files shortly to include the Elo ratings for the teams in each match also.

Please feel free to use these Elo ratings in your work, should they prove useful. If you do, please cite the following:
"Developing Elo Ratings for Club Football Matches”, Reade, J.J., De Angelis, L., and Singleton, C., 2026, Discussion Paper, Department of Economics, University of Reading.
