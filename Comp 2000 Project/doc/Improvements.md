
improvement 1: implemented a function that closes the game as the players health reaches 0, before the fix nothing happened when health reached 0 and continued to -5000 so health was irrelevant. this is done on line 34 of main by ending the java application once player.damage reaches 0. this saves the user the effort of manually closing out of the game once its over.

improvement 2: implemented a fuction that closes the program if the game is won (all items collected without dying), previosly the game would freeze and the player had to close the game manualy. implemented on line 38 of main.

improvement 3: by  decreasing time between measuring user inputs(line 126 of main) the game can run alot smoother with less hitching and stuttering


improvement 4: i increased the difficulty of the game by adding extra enemies for the user to avoid. this was done by changing the data in stage1.map on lines 6,7,8.