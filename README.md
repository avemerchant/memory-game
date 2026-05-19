# memory-game
This is a collection of files that I made for the sake of a homework assignment for CSC 276: Object Oriented Software Design. The instructions were along the lines of: Create a memory game that is played with tiles that each have 2 sides. The memory game starts with a board of 4x4 tiles. Extra Credit: Allow the user to choose the level of difficulty. This project and game were created using Java FX and model view controller architecture. 

The total instructions for this assignment are as follows: 
In this assignment you will create memory game using Java FX and you design your implementation using the model view controller architecture. 

1. Requirements of the Memory Game
The memory game is played with tiles where each tile has 2 sides. All tiles have the same generic symbol e.g. ? (or an image) on one face but each tile has a different value or image on its face up side. The memory game starts with a board of 4x4 tiles. All tiles are initially placed face down. The board contains pairs of tiles with matching values on their face up sides. The tiles are randomly placed on the grid and the goal is for the player to find the tiles which match and pair them up. Gameplay: On each turn the player chooses one tile and the tile is flipped over. Then the player chooses another tile which is also flipped over. If the tiles have matching face images they form matched pair and can no longer be selected by the player. If the two tiles don’t match they are both flipped faced down again. It is important to have a bit of a pause to allow the player to see the facedown values of the tiles before they are matched or flipped over. This allows the player to memorize the values or to verify whether they matched. The game moves to the next turn. The goal is to form matched pairs for all the tiles. When all tiles are matched up the application should ask the user if they like to play again and if so the board should be re-initialized and all tiles be enabled to be selected by the user.

2. Requirements for Design
The model view controller architecture must be used. You must explicitly use the words Model, View and Controller in the names of your classes e.g. MemoryGameModel. Your design should adhere to and will be assessed using the 276Rubric.

3. UML Class Diagram
Document your solution using a UML class diagram showing all classes and relationships between the classes. Show the names of the interfaces and super classes that each of your classes extends or implements. Please ensure the diagram is legible. If in doubt create electronically using draw.io or google drawing.

4. Grading and Submission:

• Code that does not compile or cannot be run will receive at least 80% off
• 45% - Implement all requirements described in this assignment
• 35% - Following all the criteria listed in the 276Rubics.pdf (Note this contains commenting and having your design match your implementation)
• 20% - UML diagram- Submit all your java code files and your UML diagram. Only java and pdf files will be accepted. Please ensure I can run your java files.

5. Suggestions:

• The TilePuzzle is a good example to use for this assignment. The GridPanel, buttons and the MVC architecture are all used in the TilePuzzle game.
• A PauseTransition can be used to pause the game after two tiles are flipped to allow the user time to look at the values. See below for an example. You will need to import import javafx.animation.PauseTransition; PauseTransition pause = new PauseTransition(Duration.seconds(2)); pause.setOnFinished(e -> { // Add other actions to perform after the pause here System.out.println("inside pause event"); }); pause.play();

7. Extra Credit (10 points)
Allow the user to choose between three levels of play. Easy will present a 4x4 board, Intermediate will present a 5x5 board and Hard will present a 6X6 board

As part of the class rubric, I also had to include comments above each of my functions that explained the purpose, inputs, and outputs of that function. All of the code in this repository are copy and pasted from files that were created using Java on Eclipse. 
