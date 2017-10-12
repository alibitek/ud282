# Tic-Tac-Toe game

### Summary

In this project, you are required to complete the code for a Tic-Tac-Toe game. The source code of the game GUI and computer logic can be downloaded here. While you can start compiling and playing straight away, the code is not complete because the game never detects the winner! 

### Rules of the Game

Tic-Tac-Toe is a 2 player board game. One player is X and the other player is O. The game starts with an empty 3x3 grid with 9 cells. The players take turns marking each cell with either an X or an O. The goal for the X player is to get 3 X’s in one line either vertically, horizontally or diagonally. The goal for the O player is to get 3 O’s in one line either vertically, horizontally or diagonally.

X wins by forming a diagonal line

O wins by forming a horizontal line

Once a line is formed the game ends and the player who formed that line wins!

Sometimes there is no winner. This occurs when all of the cells are filled in but there is no line of 3 X's or 3 O's. This often happens, especially when both players are good. In this case, this game ends as a tie.

Game ends as a tie

### Code design

The source code includes 2 main Java files, Game.java and GameUI.java.

    Game.java is where all the game logic code exists.
    GameUI.java is where all the user interface code exists. You can take a look at GameUI.java if you like, but it is not necessary to change any code there to complete the project.

Your job is to implement the checkGameWinner() function in the Game.java file.

String checkGameWinner(char [][] grid) has a 2D char array as an input representing the game grid (see below for details) and it returns a String message indicating which player has won (X wins , O wins, Tie, or None if the game hasn't ended yet)

doChecks() is another function that is responsible for calling checkGameWinner every time a player takes a turn, so you should not worry about fitting this function into the rest of the program, this is already taken care of.

The Grid is represented as a 2D array of characters, indexed as follows:

2D Array Indicies

### Requirements

In checkGameWinner() you should access those cells in the 2D array to find out if X or O has won the game by checking if there’s 3 of the same kind in a row either horizontally, vertically or diagonally!

    If you detect a winner, set the variable result to either “X wins” or “O wins” depending on the player who won.
    If the game ends as a tie, set result to “Tie.”
    If the game has not ended yet set result to “None.”

Then make sure the function returns that variable result at the end (you can also return the string literal directly as you detect a winner or tie).

You are allowed to create and use extra functions if you want, but you should not need to do so.

As a free student, you will not be able to submit your project to Udacity for review. Make sure you test the code by playing the game many times with different outcomes (X wins, O wins, tie). If you find a bug, remember that you can use the debugging feature in IntelliJ to point you to the right direction. Check the forums for help from your fellow students.

Good luck! We hope you enjoyed taking this course.

### Test
./gradlew clean test
