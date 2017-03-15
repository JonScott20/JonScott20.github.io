---
layout: page
title: Class Work
permalink: /class_work/
---

Course Work from the California Polytechnic State University, San Luis Obispo

All of my work done as a student at Cal Poly is covered under a collaboration agreement. 
In order to promote academic honesty, I am only willing to share code samples from the projects when contacted individually.
Project specifications are also availabe upon request.

**CPE 357 - Systems Programming**
------------------------------------------------------------------------------------------------------------------------------
Kurt Mammen Winter Quarter 2017
Course Description: C programming language from a system programming perspective. Standard C language including operators, I/O functions, and data types in the context of system functions. Unix commands, shell scripting, file system, editors.

**Project 1 - Mastermind**
------------------------------------------------------------------------------------------------------------------------------

Wikipedia explanation of the [Mastermind](https://en.wikipedia.org/wiki/Mastermind_(board_game))
  
**Project 2 - Word Count**
------------------------------------------------------------------------------------------------------------------------------


**Project 3 - Word Frequency**
------------------------------------------------------------------------------------------------------------------------------

**Project 4 - Battleship**
------------------------------------------------------------------------------------------------------------------------------

This was by far my favorite project of the class. It was an exercise in using fork, exec in order to create multiple processes and pass information between them via pipes in order to create a simulation of the classic Battleship board game.

The class was then given the opportunity to create a player to compete in an optional tournament against the rest of the players in the class for additional credit. Of 105 people in two sections of the class, only around 30 people qualified to compete in the tournament. The image below is how I ranked among those who qualifed. My username is Jscott24, highlighted green. The instructor joined in the fun too - his username was kmammen, highlighted blue.


![Project 4 Tournament Results](https://jonscott20.github.io/Files/Documents/Project4Tournament.png)


**My strategy**

I decided that I would get the most benefit from focusing on the offensive part of the game. I chose to break down how the next shot was selected into two modes: mode 1: hunt and mode 2: destroy. I referenced a post on [datagentics.com](http://datagenetics.com/blog/december32011/index.html) in order to design my strategy. 


**Hunt Mode: **
The hunt mode takes advantage of the parity in a 10x10 standard battleship board. Even the smallest ship, the patrol boat, must occupy at least one even parity square. So I created a list of all even squares and worked my way through the list until getting a hit, which would trigger the destroy mode. Instead of starting in a corner, I chose to start shooting at squares in the middle of the board and work my way out in a clockwise fashion. 


**Destroy Mode: **
Everytime a hit was registered, all the surrounding squares that immediately bordered the hit location (excluding diagonals) were to be pushed onto a stack data structure. Successive shots were the popped off the stack and checked for validity (not out-of-bounds and the square as not already been shot at) until no further shots remained on the stack, and the player returns to hunt mode.

**If there was more time...**

I would have liked to beefed up the defensive capabilities of my player. As it was, I created three different boards and merely cycled through them after each game. A random placement of ships would have been a good counter to any shot history implementations my opponents may have used. 


  
**Project 5 - C Shell**
------------------------------------------------------------------------------------------------------------------------------

**Project 6 - LZW Compression**
------------------------------------------------------------------------------------------------------------------------------

The LZW compression algorithm paired with bit packing and recycling with codes between 2^9 and 2^15

