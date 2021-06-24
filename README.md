# MultiThreaded-Ludo
Multi Threaded Ludo Game with a well commented simplified code using semaphores and OpenGL Glut library.
Ludo is a strategy board game for two to four players, in which the players race their
four tokens from start to finish according to the rolls of a single dies. This project
consists of designing a multithreaded application of Ludo for four players each having
maximum four tokens. Two, three or four can play, without partnerships. At the
beginning of the game, each player’s tokens are out of play and staged in the player's
yard (one of the large corner areas of the board in the player's color). When able to, the
players will enter their tokens one per time on their respective starting squares, and
proceed to race them clockwise around the board along the game track (the path of
squares not part of any player's home column). When reaching the square below his
home column, a player continues by moving tokens up the column to the finishing
square.
The rolls of a single die control the swiftness of the tokens, and entry to the finishing
square requires a precise roll from the player. The first to bring all their tokens to the
finish wins the game. The others often continue play to determine second, third, and
fourth place finishers.
Design:
  1.Each player rolls the die.
  2.Players do not take turns sequentially i.e. players alternate turns in a random fashion.
  But for each round of rolling the die to be complete, each player needs to complete
  his turn.
  3.To enter a token into play from its yard to its starting square, a player must roll a 6. If
  the player has no tokens yet in play and rolls other than a 6, the turn passes to the
  next player. Once a player has one or more tokens in play, he selects a token and moves it forwards along the track the number of squares indicated by the die.     Playersmust always move a token according to the die value rolled
