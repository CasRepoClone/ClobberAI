# ClobberAI
**minimax and alpha-beta pruning for AI move prediction on the board game 'Clobber'

_Originally, game was designed on a 5x6 board, but more and more games are
being played on a 10x10 board. Each player has his own color. At the beginning,
the board is completely covered with disks, so that black disks are placed on
black fields, and white disks are placed on white fields. A black player starts the
game. Players move alternately. The move can only be made to a orthogonally
adjacent space occupied by the opponent’s disk. Once the move is made, the
opponent’s disk is "clobbered"and removed from the board, and the player’s
disk takes its place. The game ends when there is no more moves for any of
players. The winner is the player that moved the last.
Using the information in this list and those given in the lecture, write a program that plays Clobber (board size nxm=5x6, can be modified). The program
should, on the standard input, accept a starting board (e.g., the default starting
3
board for the Clobber game), allow the selection of heuristics, and adjust the
parameter d which is the maximum search depth of the decision tree. The board
representation should has the form of m lines consisting of n space-separated
marks – B denotes player one’s disk, W denotes player two’s disk, _ denotes
an empty field. Player ones’s turn follows._

The Minimax algorithm is a game tree search strategy that is used to make
decisions in two-player zero-sum games such as chess, checkers, and go. The
algorithm seeks to minimize the maximum possible loss a player can suffer,
given the opponent’s moves. The Minimax algorithm is based on viewing the
game tree, where each vertex of the tree represents a game state, and the edges between them represent the players’ moves. The leaves will be the vertices
representing the end of the game won by one of the players. In practice, due
to the number of vertices increasing exponentially with depth, we use a depth
limit and heuristics for evaluating the game state, allowing us to evaluate the
unfinished game if we reach this limit

The alpha-beta pruning algorithm is an extension of the Minimax algorithm,
which allows you to skip considering unnecessary nodes in the game tree and
2
thus reduce search time. The alpha-beta pruning algorithm works by eliminating branches of the tree that are certainly not optimal, as they contain only
moves that will not improve the value function for a given node. This algorithm
significantly reduces the number of nodes that must be browsed when searching
the game tree.
