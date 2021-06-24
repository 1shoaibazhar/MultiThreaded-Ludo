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
  
  3.To enter a token into play from its yard to its starting square, a player must roll a 
  
  4. If the player has no tokens yet in play and rolls other than a 6, the turn passes to the
  next player. Once a player has one or more tokens in play, he selects a token and moves it forwards along the track the number of squares indicated by the die.     
  5.Players must always move a token according to the die value rolled.
  Passes are not allowed; if no move is possible, the turn moves to the next player.
  
  6.A player will keep on throwing the dice if Six comes.
  
  7.Three consecutive sixes will result in loss of turn and all his numbers in that turn will
  be discarded.
  
  8.When a 6 is rolled, the player may choose to advance a token already in play, or may
  enter another staged token to its starting square. Rolling a 6 earns the player an
  additional or "bonus" roll in that turn. If the bonus rolls results in a 6 again, the player
  earns an additional bonus roll. If the third roll is also a 6, the player may not move and
  the turn immediately passes to the next player.
  
  9.Players may not end their move on a square they already occupy. If the advance of a
  token ends on a square occupied by an opponent's token, the opponent token is
  returned to its owner's yard. The returned token can be reentered into play only when
  the owner rolls a 6.
  
  10.There are some "safe" squares on the game track which protect a player's tokens from
  being returned. They are shown in the board with player colors. A player's home
  column squares are always safe, however, since no opponent may enter them.
  
  11.If a piece lands upon a piece of the same color, this forms a block. This block cannot
  be passed or landed on by any opposing piece.
  
  10.When a piece has circumnavigated the board, it proceeds up the home column. A
  piece can only be moved onto the home triangle by an exact throw.
  
  11.A player should not be allowed to enter into his Home column until he has removed
  at least one opposing piece.
  
  12.The first person to move all 4 pieces into the home triangle wins.
