# Analyzing-The-Effects-of-Environmental-and-Situational-Factors-on-Yardage-in-NFL-Rushing-Plays

**Introduction**

Over the past several years, the NFL has grown increasingly interested in statistical analysis and big data, and
how statistics can potentially affect how the game is watched and played. And, while they have now begun
to collect game data, the NFL still has a shortage of statisticians to actually analyze it. Due to this, the NFL
conducts an annual Big Data Bowl, a competition open to the public, where the organization provides game
statistics from previous years, and the group with the most accurate predictive model is awarded $75,000
dollars. This year’s Data Bowl revolves around the prediction of a rushing play’s expected yardage, given a
multitude of variables such as, but not limited to, player, offensive formation, and weather.

The dataset from this study is found on the NFL’s Kaggle Big Data Bowl website (https://www.kaggle.com/
c/nfl-big-data-bowl-2020/data). The dataset contains 23,171 observations of 49 variables, one for each player
present in each rushing play from the 2017 and 2018 seasons. Unlike most sports that are played either inside
or during warm seasons, football is in the unique position of being a primarily outside sport that also combats
the harsh weather conditions that come with Fall and Winter. Potential snowfall or high windspeeds could
completely alter how a football team plays the game. In general, the environment a game takes place in may
affect a rushing play’s yardage. For the purposes of this study, there are six intriguing predictors that may be
derived from the dataset that can be deemed “environmental”: the game’s weather, the game’s temperature
(deg F), the game’s humidity, the game’s wind speed (in miles/hour), whether the game was played on turf
or grass, and whether or not the offensive team has home-field advantage.

In addition to environmental factors, another interesting aspect to the NFL is how fluid the game is. For
example, depending on the quarter, down, yards needed for a first down, yards needed for a touchdown, and
current point difference between the offensive team and their opponent, a play could essentially already be
decided before it is even run (and the defense could be ready for it). Therefore, the goal of this analysis is
to see if rushing plays are best predicted using constant factors (such as environmental factors that persist
throughout the game), situational factors, or some combination of both. While situational factors are unknown
before the onset of the game, constant factors such as weather can be accurately predicted days before, and
therefore could be more assuredly used in pre-game preparations if the analysis deems the factors to be
significant predictors. If it is indeed more relevant to use situational factors as predictors, much is revealed
about the fluidity of a game and which situations lead to optimal and suboptimal rushing plays.

In order to accomplish this task, separate linear regression models will be run to infer feature significance
as well as the strength of the models in explaining the variance in the yardage gained in a play. The first
will use only constant factors to predict yardage. The second will only use fluid factors. And the third and
subsequent models will build off the first two to try and create the best prediction model for rushing yardage
using constant and/or fluid factors.
