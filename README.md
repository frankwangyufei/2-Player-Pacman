# 2-Player-Pacman

This is a self-proposed project by Wang Yufei for the COMP2611 course offered by HKUST in 2018 spring.

# Feature
This is a two player pac-man game. 


# Controls
First player: wasd

Second player: ijkl


# Rules
1. Pacmans could not intersect each other
2. Pacmans could acquire score by touching score point objects
3. Any pacman that come into contact with a ghost will enter quiz mode
4. Quiz mode
	1. Once on quiz mode, a question and 4 choices will appear, enter answer using 1234.
		1. If the answer is correct, the pacman triggering the quiz will be teleported into a cell without ghost
		2. If the answer is wrong, both pacmans will enter "shield mode", with the pacman triggering the quiz frozen in place until the shield_alert_time is reached
5. Shield mode
	1. In shield mode, pacmans could intersect each other (this override rule 1)
	2. In shield mode, pacmans could pass through ghost freely (this override rule 3)
6. End of Level
	1. The end of level is reached when all score points are collected
	2. The end of level would reset score points, score, and pacman positions
7. End of Game
	1. The end of game is reached when level 2 is passed
	2. The winner of the game would be the player with the highest cumulative score in level 1 and 2
