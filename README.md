Download Link: https://assignmentchef.com/product/solved-cs161-week-9
<br>
Write a class called Board that represents a tic-tac-toe board.  It should have a 3×3 array as a data member, which will store the locations of the players’ moves.  It should have a default constructor that initializes the 3×3 array to being empty.  It should have a method called makeMove that takes the x and y coordinates of the move (see the example below) and which player’s turn it is as parameters.  If that location is unoccupied, makeMove should record the move and return true.  If that location is already occupied, makeMove should just return false. There should be a method called gameState that takes no parameters and returns one of the four following values: X_WON, O_WON, DRAW, or UNFINISHED – use an <strong>enum</strong>​          for this, ​     <strong>not</strong>​        <strong> strings</strong> (the enum definition should go in Board.hpp).  There should also be a method called​            print, which just prints out the current board to the screen.

Write a class called TicTacToe that allows two people to play a game.  This class will have a field for a Board object and a field to keep track of which player’s turn it is.  It should have a

constructor that takes a char parameter that specifies whether ‘x’ or ‘o’ should have the first move.  It should have a method called play that starts the game.  The play method should keep looping, asking the correct player for their move and sending it to the board (with makeMove) until someone has won or it’s a draw (as indicated by gameState), and then declare what the outcome was.

Write a main method (in TicTacToe.cpp) that asks the user which player should go first, creates a new TicTacToe object and starts the game.  ​<strong>For this assignment only, you will not comment out your main method. </strong>

Input validation​<strong>:</strong>​ If someone tries to take an occupied square, tell them that square is already occupied and ask for a different move.

Here’s an example portion of a game (already in progress):

<ul>

 <li>1 2 0 x . .</li>

 <li>. . .</li>

 <li>. . .</li>

</ul>




Player O: please enter your move.

1 2




<ul>

 <li>1 2 0 x . .</li>

 <li>. . o 2 . . .</li>

</ul>




Player X: please enter your move.

1 2

That square is already taken.




0 1 2

<h2>0 x . .</h2>

<h1>1 . . o</h1>

<h2>2 . . .</h2>




<h1>Player X: please enter your move.</h1>




The files must be named: ​<strong>Board.hpp</strong>, ​ ​<strong>Board.cpp</strong>​, ​<strong>TicTacToe.hpp</strong>​ and ​<strong>TicTacToe.cpp </strong>