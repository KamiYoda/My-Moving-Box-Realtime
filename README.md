# Welcome to My Moving Box Realtime
***

## Task
The problem was to complete an index.html file which had missing javascript code for the movement of it's <div>

with the id ='my_box_realtime' from it's original coordinates to the given coordinates(right = 0 & bottom = 0)

## Description
I defined two variable x,y to denote the right and bottom(horizontal and vertical axis) respectively, also with 

another variable named start_moving to hold the setInterval() command and another named my_box to hold the <div> 
element meant to be moved.

I then created a function move_diagonal which housed two if statements the first with the condition (x && y < 70) 

in which if met the program proceeds to carry out the commands
          my_box.style.right = x + 'px';
          my_box.style.bottom = y + 'px';

          if (x <= 70 && y <= 70){
              x--;
              y--;
               
within the first if statement and the second which had the stopping condition of if (x && y == 0)
it clears the interval with clearInterval(id)



## Installation
No Installation needed for this project

## Usage
It works by the function setInterval() making a function call on move_diagonal method which in turn 

causes the method to execute its statements until the specified coordinates of x && y == 0 is reached

which in turn calls the clearInterval() function and brings the movement to a halt at the coordinates 

x = 0 and y = 0

