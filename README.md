# footycomp
URL: https://footycomp.streamlit.app/

Import your own player dataset and create pizza/radar charts and compare players for chosen stats.

Requirements to upload dataset: Player (Name), Nation, Team, and Position columns exist.

This streamlit app uses any dataset you provide utilizes the mplsoccer package to create Pizza and Python charts of the players alongside tables for similar players and best players per position based on chosen stats.

The user can provide a player (or two for comparison pizza chart) and the position they want to analyze the player's statistics with respect to other players in the position via percentiles. They can also select to use either a radar or pizza chart if only looking at one player, but for comparing two players a pizza chart will be selected by default as that is currently the only option for comparison. The user can also select the number of players they want to compare with the chosen player via a slider which will then create a table displaying the chosen amount of the most similar players and their respective critical stats based on the position chosen. There are also nation and team filters that restrict the set of players to start from before performing the percentile calculations. Finally, the user can choose a position and set of stats (along with the team and nation filter from the similar players) to view the best players according to those stats using average percentile.

You can now select whatever stats you want to compare for the chosen position with the Stats dropdown in the sidebar.

It should be noted that inverse percentiles for errors and goals allowed related stats are used as for those stats, lower values indicate better performance overall. You can add stats to be considered as such under the optional filters.
