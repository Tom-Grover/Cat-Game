
Stage:
from line 70 to line 89 of stage a new thread is created each time a different actor is called. this means that the movement calculations for the actors are all happeneing in parrallel. this was done by adding a lambda( new Thread(() -> { ) at the start of the function and .start(); at the end to begin using a new thread for wverythin in between these 2 points. the reason for running all of the actors on seperate threads is that it allows the game to calculate their movement all at the same time while using much less rescourcess then doing all of the calculations after each other.

Cell:
on lines 29 - 31 a new thread is created every time an actor is painted. on line 28 it checks if an actor occupies the cell, if an actor occupies the currently checked cell it creates a new thread by using the lambda new Thread(() -> {. the thread will then be instructed to draw the actor using paint on line 30. on line 31 .start() is used to finish defining the threads activities and actually begin them.

