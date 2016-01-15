# VORP Project for CSC 121

Source: <b><cite>Introduction to Algorithms</cite></b> by Thomas H. Cormen, Charles E. Leiserson, Ronald L. Rivest, and 
Clifford Stein, The MIT Press, 3rd edition, 2009, ISBN-13: 978-0262033848

<b>Problem 15-12 (Signing free-agent baseball players)</b>: Suppose that you are the general manager for a major-league
baseball team. During the off-season, you need to sign some free-agent players for your team. The team
owner has given you a budget of $X to spend on free agents. You are allowed to spend less than $X
altogether, but the owner will fire you if you spend any more than $X.

You are considering N different positions, and for each position, P free-agent players who play that
position are available.  Because you do not want to overload your roster with too many players at any
position, for each position you may sign at most one free agent who plays that position. (If you do not
sign any players at a particular position, then you plan to stick with the players you already have at that
position.) To determine how valuable a player is going to be, you decide to use a sabermetric statistic
known as “VORP,” or “value over replacement player.” A player with a higher VORP is more valuable than
a player with a lower VORP. A player with a higher VORP is not necessarily more expensive to sign than a
player with a lower VORP, because factors other than a player’s value determine how much it costs to
sign him. For each available free-agent player, you have three pieces of information:

    • the player’s position,
    
    • the amount of money it will cost to sign the player, and
    
    • the player’s VORP.
    
Devise an algorithm that maximizes the total VORP of the players you sign while spending no more than
$X altogether. <s>You may assume that each player signs for a multiple of $100,000</s>. Your algorithm should
output the total VORP of the players you sign, the total amount of money you spend, and a list of which
players you sign. Analyze the running time and space requirement of your algorithm.

Sabermetrics is the application of statistical analysis to baseball records. It provides several ways to
compare the relative values of individual players.

-------

Your program should be written in Python and should be able to read and process the (2015) real previous salary data from http://sports.newsday.com/long-island/data/baseball/mlb-salaries-2015/ , available in the file salaries.txt and the previous VORP data from http://www.baseballprospectus.com/sortable/index.php?cid=1819072 , available in the file vorp.txt.  You will need to figure out how to get and combine the relevant data from the two files (player, position, vorp, and salary).

As a couple of test cases:

A budget of 5000000 should yield the following results:

> Team: Devon Travis, Joc Pederson, Mark Canha, Chris Dominguez, Matt Duffy, Paulo Orlando, Nick Ahmed, Roberto Perez, Randal Grichuk

> Total VORP: 152.9

> Money Spent: 4572500

A budget of 10000000 should yield the following results:
> Team: Devon Travis, Joc Pederson, Mark Canha, Chris Dominguez, Matt Duffy, Jorge Soler, Daniel Norris, Nick Ahmed, Roberto Perez, Randal Grichuk

> Total VORP: 157.3

> Money Spent: 7240367

<b>You should fork this repository.</b>

