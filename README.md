RobotJS
========

Node.js GUI Automation. Control the mouse, keyboard, and read the screen.

This is a work in progress so the exported functions could change at any time before the first stable release (1.0.0). 

Based on [autopy](https://github.com/msanders/autopy). 

##Installing##
```
npm install robotjs
```

##Examples##
Get the mouse location and move it. 

```JavaScript
var robot = require("robotjs");

//Get the mouse position, retuns an object with x and y. 
var mouse=robot.getMousePos();
console.log("Mouse is at x:" + mouse.x + " y:" + mouse.y);

//Move the mouse down by 100 pixels.
robot.moveMouse(mouse.x,mouse.y+100);

//Left click!
robot.mouseClick();
```
##Progress##

| Module        | Status        | Notes   |
| ------------- |-------------: | ------- |
| Mouse         | 80%           | Can't specify mouse button.       |
| Keyboard      | 50%           | No toggle support.       |
| Screen        | 5%            | Screenshot, read pixel color, image search.        |
| Window        | 1%            | Manipulate external windows.     |
