# Project Report

### I. Initiative
The project is a game that is based on a non-playing character - NPC, targeting and chasing the user's cursor. The NPC is a character controlled by the computer. It will target the users mouse position as the player moves across the screen. The game is over once the NPC touches the players mouse position 3 times. The user then has a option of restarting the game but clicking on the button 'Restart'
### II. Epics and User Stories

##### Epics

The main fucntion of the game will be the user input the mouse's cursor into the canvas area to start the game. Then have the game be triggered from this action. This trigger will start the startGame fucntion. This function will load the two rectangles that are under two different functions: "myGamePiece" and "myEnemyPiece". 

"myGamePiece" will be the rectangle / square the user controls. This will be controlled by using cordinates in the code, as the cordinates will be set to where the cursor is on the screen. The corodinates set the basis for the rectange to be whereever the mouse is. 

"myEnemyPiece" is the computer controlled rectangle / square. This will be the same width / height but will be different colour. This will be following the user's cursor by having an equation that allows the square to start of at a different set or cordiantes and will use speed to follow the cursor. The NPC will be following the cordinates but will using speed to dertmine the pace of the game - if the NPC is chasing the user's square fast or slow. Once the NPC has touched the user's piece three times, the game will be over. The user can then click on the 'restart' button to trigger the startGame fucntion.


##### Non-Functional Requirements

Within the game there are Asthetic and / or non essential requirements. These often include features of the objects that do matter but are not a whole fucntion on their own: heigh on objects, the width, the colour - defined often through the use of html colours black being #000000, the type of shape (round or Rectangular...), the border outline colour, the colour of the canvas, the padding... These are all Asthetic pieces that belong in a function, that will create the function. A button will be included to allow the player to restart the game and keep playing. Text will also be displayed to welcome theplayers to the game.

##### User Stories

As a player, I would like to be able to move the shape with the cursor and have the square where every the mouse is. The shape shouldn't be creating a drawing effect on the page or be just off with the cursor.

I would like to see an opponent shape that once the games start follows the shape im controlling; with a certain speed with the movement.

As a player, I would like to see a score or a counter for how many lives that I have left. 

As a player, i would like to see some text welcoming me to the game.


##### How We Addressed The Requirements

The first step was to assess the brief requirements and break down what must be included. The brief states:

A non-playing character NPC (that is a character controlled by the computer) targets the users mouse position as the player moves across the screen, the game is over once the NPC touches the players mouse position 3 times. 

When breaking down the requirements, it is known that a NPC has to be included. This can be in the form of a square or rectangle and the diameters havent been speficied, nor has the location of the NPC. 

It is known that the NPC has to chase the cursor some research into javascript will be made to figure out the function that will allow the NPC to chase the user's mouse. This is going to have to include the use of cordiantes and a delay that uses speed within. 

A playable character is going to have to appear as a different colour shape than the NPC. The playable character will have to follow the current movements of the cursor. It cannot be delayed or create a drawing onscreen. The playable character has to follow the cursor by using the cordinates.

If the NPC touches the playable character then the game will start again until the NPC has touched the playable three times. Once this occurs the game is over. There has to be a score variable that stores the amount of times the NPC has touched the other. Then there has to be an if statement that stops the objects from moving once that score has been reached. However, this is not a must as the brief didn't specify they want a score board or life counter.

A button will be included to restart the game. This will be an event listener that once clicked on will restart the game. This will use the function startGame.

### III. Genre

The genre of this project is that it is a casual 2D reaction game. This is due to the user having to navigate the playable character from the NPC. This type of genre suits the games reqiurements as there isn't much depth in the game itself.

### IV. Technical Details

##### Platform

The best platform for this project on is Chrome. This is because it has the most up-to date html version within. Chrome supports alot more of the features than other web browsers. For example when trying to load the project onto internet explorer the project doesnt even load, only the text does. Whereas Chrome loads the whole project. It allows the complete project to use the HTML file, Javascript and CSS files with little issues.

##### Programming Language/Enviroment

The envrioment / programming languages used were HTML, Javascript and CSS.

Hypertext Markup Language is the language used to describe the overall struture of the webpage. It is the building blocks of HTML pages as it uses the elements within. It allows the elements to be easily idenified as tags and HTML allows tags to have appropriate labels: "headings", "body", "font"... Then these tags create the ability for the content to be fully rendered. 

Javascript is used to help with the real time interactions that are going on in the webpage. This is used to read the script in the code and render the results. This is often for the use of the client side.

Cascading Style Sheets (CSS) is a style sheet programming language that will describe the style of HTML webpage. It describes how the elements within need to be displayed. It is the presentation of a document in HTML. It allows the webpage to adjust to the devices in use; it adjusts to bigger and smaller screens.

##### Programming Challenges

The first issue I had was identfying specific issues. As I was in notepad, this didn't have a process that made debugging alot harder. To solve the issue i had to debug the programm in the webbrowser, this would only show syntax errors. Making it lack any IDE, whcih would have shown each section of the code.

The second issue I had was making the enemy appear in the canvas and making it actually appear as if it was chasing the cursor. IT would either not appear in the canvas area, chase the cursor or it would load on top of the playable character.

Figuring out how to track the amount of lives the user has and the score the user has.

 
##### Constructing And Implementing My Code

Think of this as the method. How will you go about building your program?


##### Algorithms

The main Algorthim that had to be used was when creating the Enemy object. This would be down to the enemy piece having to be able to chase the user's cursor cordinates. The algorthium is broken down into a procedure and will be broken down into each step. Each step will have a goal that if done correctly, will produce an outcome.

When the user moves their piece the algorith is triggered. The algorithm should have the enemy square towards the user's piece. When the user move to the right of the canvas the enemy has to go to the right. (vice versa). This is creating the illusion that the emeny piece is chasing the user's piece. The algorthim also has to include speed. This as the enemy has to chase the user and not teleport to the user's cursor immediately.
 
##### Coding Standards 

The standards of code that will be used need to be harmonised, consistent and in a coherent style. The coding standards that are fundental are the Good Basic Standards. These will be used to the best ability. The main focus are on:

The layout of the code

The name of the functions and variables are strutured well

Making sure that the code is readable and is understood.

### V. Research

Research found was from www.w3schools.com. Specifically the HTML, JavaScript and CSS pages were used as a guidence.

### VI. Project Management

##### Burndown Chart

![](https://github.com/AoifeW123/Tracerball/blob/master/Burndown.jpg)

This chart shows the what days were spent working. This is shown in the blue, the orange shows the days that were expsected.

##### User Stories Tracking Chart (Which Stories Have Been Completed)

Table showing user stories with weighting, due date and completion state

![](https://github.com/AoifeW123/Unit-1-Programming/blob/master/Implimented.jpg)

the one should represent a no not yes


##### Flowchart

Flowchart showing how the program will work

##### Functions

Descriptions of functions given on flowchart
