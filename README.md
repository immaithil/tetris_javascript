# tetris_javascript
This is a famous brick game tetris made using vanilla javascript https://sad-swanson-c56815.netlify.app/

## Description
It is an amazing and simple game invented by Alaxy Pajitnov in year 1984. I created a replica of that game using JavaScript HTML and CSS. In this game random 4 box structure fall form up and we have to stack in such a way so that it can fill the whole row. After filing a whole row that row get cleaned and it keep going until u touch the top of board.
This board can be said as a 2D matrix with 20 rows and 10 columns. 

## project construction
I first created the skin of board in classical brick game console which we used to play in our childhood. For creating the board I used canvas element of HTML as drawing structures is easy in it. I converted the canvas element to 20*10 matrix board.Then created all the 5 kind of structures and all of their orientation inside a 3D matrix which is stored inside tetrominoes file. The code for game is in tetris.js file and remaining files are sound effects I used in this game.

## game animation
Initially I tried to use set Interval for animation but I found that brower doesnt behave well with timer functions, so I later used three variables now, delta, and speed so now records the time at which a tetromino drops, delta records the current time and speed is the time differance after which the tetromino drops again. Then used the function request animation frame which will run the drop function as animation untill it collides with another tetromino or base of the game board.

## game functions
There are total 7 working keys in the digital console one key with (+) notation is uses the function level up which increases the speed of game and add the level same with (-) key except it decreases the level. Then there is R key which reset or restarts the game. There are 4 console key in which the up key is linked with rotate function and it rotates the tetrominoe in clockwise direction every time we press it. The left key linked with move left function the right key linked with move right and the down key is with move down function. I have added an extra function kick which will kick the tetromino back if we want to rotate it when it is touchin 1st or last column  of the board.

## Sound effects
I have borrowed sound from https://www.findsounds.com/ISAPI/search.dll?keywords=tetris this site and used play function which is also linked with keys.

## summery
This is a simple yet exciting game. I hope u will like it. Thanks 
