The given webpage displays a canvas with gray background and brown ground. In this lab, you will write the necessary JavaScript to create the snowman scene shown in the example image.

Task 1: Inspect the project
The index.html file contains a single 300 x 300 canvas. 

The snowman.js file contains three completed functions:

The DOMContentLoaded event handler calls drawGround(), drawSnowText(), drawSnowman(), and drawSnowflakes() to create the snowman scene.

drawGround() displays brown ground under a light gray sky.

drawSnowflakes() calls drawSingleFlake() 100 times to display 100 snow flakes in randomly chosen locations.

Task 2: Implement drawSnowText()
The drawSnowText() function should display the string "SNOW" using:

font: 80px Verdana
textAlign: center
textBaseline: top
fillStyle: blue
fillText()to display the text at coordinate (canvas.width / 2, 10)
Task 3: Implement drawSnowman()
The drawSnowman() function should display three white circles:

Bottom circle: arc() centered at (150, 200) with radius 50 that begins at 0 and ends at Math.PI * 2
Middle circle: arc() centered at (150, 120) with radius 40 that begins at 0 and ends at Math.PI * 2
Top circle: arc() centered at (150, 60) with radius 25 that begins at 0 and ends at Math.PI * 2
All three circles should use fillStyle white and be displayed with the fill() function
Task 4: Implement drawSingleFlake()
The drawSingleFlake() function should display a single white snowflake in the shape of a diamond using the constant flakeSize:

Start a new path
Move to the coordinate (x, y)
Draw a line to (x + flakeSize / 2, y + flakeSize / 2), then to (x, y + flakeSize), and then to (x - flakeSize / 2, y + flakeSize / 2)
Use the fillStyle #eee
Use fill() to display the diamond