Robot Simulator!

Requirements:
    - A web browser running javascript
    - probably computer, display, a mouse and keyboard (but if you're reading this you already have it!)

To run:
    - Run the robot-simulator.html file after downloading!

The database (which is just a 2D array), rule base (just a bunch of if/elses), inference engine (see code for simulation details) is all programmed in Javascript.
In addition, because it's javascript, all graphics elements are just CSS + HTML. File IO is handled by the browser, along with any other system IO.

A log is displayed on the right side of the page, indicating actions taken, along wiht allowing user to:
* import/export their custom grid, 
* dump robot memory, 
* view what the optimial solution would be if everything is known from the beginning (via Dijkstra's)
* reset ending or starting points (or everything)
* randomly generate obstacles
* set the starting position's heading 

Simulation and Dijkstra's requires that a start and end point be specified. 

Finally, the robot only has the following moveset;
1. Robot can go forward (not altering it's heading)
2. Robot can steer forward towards it's left (changing it's heading -45 degrees)
3. Robot can steer forward towards it's right (changing it's heading +45 degrees)
4. Robot can reverse (not altering it's heading)
5. Robot can rotate in place (either left or right, -45/+45 degrees)