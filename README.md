# Chutes-and-Ladders

Chutes and Ladders

Description

A popular board game for children is called "Chutes and Ladders". The board has squares which are numbered from 1 to 100, and players have counters which start on the theoretical square 0. The players take turns at throwing a die with the numbers 1 to 6 on it, and each moves his or her counter forward the number of squares corresponding to the number on the die (the square they reach is found by adding the die number to the square number their counter is on). The first person to reach square 100 is the winner. 
The interest is caused by the fact that pairs of squares are connected together by "ladders" (which connect a lower-numbered square to a higher-numbered square) and "chutes" (which run from high to low). If a counter lands on the start of a chute or ladder (i.e., this is the square reached after throwing the die), then the counter is moved to the corresponding square at the end of the chute or ladder. Note that landing on the end square of a ladder or a chute has no effect, only the start square counts. Furthermore, there are some squares such that if a player's counter lands on them, then the player must either miss the next turn, or immediately throw the die again for another turn, depending on what is written on the board. A miss-a-turn or extra-turn square is never the start or end of a ladder or chute. If a player is on square 95 or higher, then a die throw which takes them past 100 must be ignored - thus a player on square 99 must ignore all throws which are not 1. 


Input

Input will start with a set of less than 1000 die throws which you must use for all games, starting each new game with the first player "throwing" the first number in the set, the next player "throwing" the second number, and so on. This set of die throws will simply be a list of random numbers between 1 and 6, separated by single spaces, with not more than 80 characters on each line. It will be terminated by the number 0. After this set of die throws, there will be one or more game sets. Each game set is in three parts. The first part is a line containing a single number giving the number of players in the game. This will be more than 1 and less than 6. Then the board is described, in two parts. The first part lists the ladders and the chutes on the board, each ladder or chute being defined on a single line. Each is given by two numbers, from 1 to 99,separated by one or more spaces. The first number gives the start square, and the second number gives the end square; so it is a ladder if the first number is less than the second number, and a chute if the order is the other way. The chute/ladder definitions are terminated by a line containing two 0's. The second part of the board description gives the lose-a-turn/extra-turn squares, if there are any. These are single numbers, one per line, defining the squares. If the number is negative, its positive counterpart is a lose-a-turn square; if positive, it represents an extra-turn square. (For example, -16 means that square 16 on the board is a lose-a-turn square, while a 25 means that players landing on square 25 must immediately roll again.) The end of this set of descriptions, and of the game description, is given by a single 0. The end of all the game descriptions is given by a game with the number of players equal to 0.

Output

Output must be one line for each game in the input, giving the number of the player who wins the game. Every game will determine a winner in fewer throws than those given at the start of the data.

Sample Input

3 6 3 2 5 1 3 4 2 3 1 2 0

2

6 95

99 1

0 0

-3

98

0

2

3 99

6 90

0 0

0

0


Sample Output

2

2
