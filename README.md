# How To Win More Games: Analyzing Rocket League Game Statistics to Improve Player Performance
This project analyzes what Rocket League players could do better in order to win more games. I gathered over 100,000 rows of 3v3 game data from high level events, from octane.gg's API, zsr.octane.gg. I investigated the difference between winners and losers using exploratory data analysis and visualizations.

I also created a logistic regression model to predict if a player will win their game based on their scoreline (minus score). For example, using the model in this project, a player with a scoreline of 4,1,1,6 (goals, assists saves, shots) has a 0.97 probabilty of winning the game, and a player with a scoreline of 0,0,0,0 has a 0.27 probability of winning the game.

The model only had an accuracy of 68%, which I believe to be satisfactory for the purpose of my analysis. Increasing the accuracy score would be difficult as there are many games where players win or lose their game regardless of their performance. For example, the player with the 4,1,1,6 scoreline ended up losing the game, and there are many players with a scoreline of 0,0,0,0 that ended up winning the game. I believe this limitation of the model is due to the games being from the 3v3 mode, where reliance on teammates performances to win the game is much higher than 2v2 and 1v1 modes.

In the conclusion of the project I wrote some tips for Rocket League players on how to they can improve their gameplay and win more games, using the visualizations and the results from the model to support them. I wrote multiple tips for each type of stat category: shots and goals, assists, saves, demos, and boost.

I used pandas, numpy, requests, matplotlib, seaborn, statsmodels, and scikit-learn to carry out this analysis.
- pandas and numpy were used for data wrangling and manipulation
- requests was used for retrieving data from the API
- matplotlib and seaborn were used for data visualization
- statsmodels was used for the logistic regression model
- scikit-learn was used for train/test splitting and evaluating the model
