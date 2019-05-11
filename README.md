# fantasy

This package contains the functions and user interface to build optimized, custom Fantasy Sports lineups for both baseball and basketball. 
It allows the user to choose between FanDuel and DraftKings for contest websites, and between NumberFire and RotoGrinders for player 
projections. Furthermore, the user can lock in or exclude certain players from their lineup. Finally, the user may request multiple lineups for multi-entry contests.

Usage:
Install the files. Then launch a Python instance and type 'import runKnap'.

Relevant Files:
- Knapsack.py: Contains implementation of a modified knapsack algorithm to optimize the lineup. Also contains functions that scrape player
projections to feed this algorithm, and to drop/lock players from a lineup.
- runKnap.py: Executes the Knapsack module with an easy to use user interface via the command line.
- Player.py: Player class for storing relevant attributes about each player.

Old Files:
- fanduel.py*: Attempt to implement automatic entry of lineups on FanDuel. Only was able to log in programatically, but could not make progress past this.
- scrapeGrind.py*: Attempt to scrape data from RotoGrinders only available by navigating tabs on the webpage (which do not change the web address). Unusable.
- testing.py: Rigorous testing module for our dynamic programming algorithm.

\* These modules require the installation of ChromeDriver in your system's PATH in order to run Selenium.

Known Limitation:
Some fantasy sports do not allow a lineup to contain more than a certain number of players from the same team. This program does not ensure that the resultant lineups observe this rule. We attempted to add functionality to check for this, but due to there not being games on the day of the submission, we were not able to test this code, and we did not want to submit any code we could not test. The code is in the program but commented out.
