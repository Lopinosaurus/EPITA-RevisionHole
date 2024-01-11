# EPITA-RevisionHole

## About this repository

This repository is a C# exercises set I made to train first year (SUP) at EPITA. It is composed of two parts (Basics and UsagiShima) which are not linked. Instructions for Basics are located in the C# source files in docstring, but UsagiShima instructions are below : 


### UsagiShima

You will implemement a UsagiShima mini-game. The main point is for you to understand how OOP works and how to create a relevant OOP architecture. In this training, we will not give you the exact instructions for every methods and functions you will code, but just the main objective of this project.
Usagi Shima, which means "Bunny Island" in japanese, is a little video game where you are:supposed to raise rabbits. You will implement a very simple version of this : 

The UsagiShima (Bunny Island) follows those rules : 
- The island is represented by a matrix of cells (board).
- Cell class is a parent class defining the global working of a board cell. Each Cell has multiple attributes (see the UML for further details).
- Each bunny needs at least one carrot.
- If there are not enough carrot, bunnies leave the island (cells are deactivated) until there are enough carrots for everyone.
- When a bunny leaves the island, it take its terrier with it. The terrier cell must then be deactivated.
- To gather carrots, the island needs carrot shops. For each lap, a single carrot shop generates 3 carrots. The carrot shop number is constant, but you can create some new rules to make it dynamic (bonus)
- At each lap, bunnies must try to move. A bunny can move if there is at least one neighbor that is not occupied (that imply diagonal neighbors).
- A board is generated by a seed. An explanation of the seed is located in `~/EPITA-RevisionHole/UsagiShima/Drawing.jpeg`
- The game stops when the board is full or when currentLap == laps.

### General Advices

You will follow the general architecture labeled by the UML. Feel free to add classes or methods if you find them relevant. At the end, your game must : 
- Follow the general rules of the game indicated above.
- You board must be printable and printed at each game turn (lap).
- Each cell should be printed with it proper color. If a cell is null or deactivated, you are free to use the color you want (as long as it is not the same colors as the active one).

The main goal is not only to follow the rules and indications for this training, but rather train yourself to be able to write some proper OOP in C#.
I strongly recommend you to send us your final (or indev) code at `louis.laverne@epita.fr` or `lopinosaurus` on discord to have a feedback and corrections.
Do not hesitate to contact us if you need help. There is nothing more deceptive than an obvious fact.

Il fait froid, prenez vos C# !



# UPDATES : 
Seed MUST BE a string and not uint.
Change uint by int in ConvertToRoman makes it easier.
