### Pattern Assignment
##### Goal
Use the basic animation code from class today, and make one of two animations:
1. An ellipse traveling along the path of a circle
2. An ellipse traveling along the path of a square
##### Submission
1. Make a 2-3 minute video explaining your code and how you approached the problem.
2. Submit a zip file of your project.
##### Hints
1. A circle, remember, has 2 pi radians. You can represent the point on a circle of radius (r) in terms of this angle. This should be 
review from Algebra 2! Remember the unit circle? You may want to store the **angle** as a class variable in your program.

```java
// Calculate the point on the circle given an angle in radians
double angle = Math.pi;
int radius = 100;
double x = radius * Math.cos(angle);
double y = radius * Math.sin(angle);
```

2. For a square, you will want to probably work with velocities (dx & dy). This will determine the direction your ellipse will go at any
moment. The velocity variables you declare will help you update you position variables to the correct values!

```java
// Declare variables to represent the x and y velocities

// Ellipse not moving
int dx = 0;
int dy = 0;

// Ellipse moving to right/left
dx = 2; //Positive for right, negative for left
dy = 0;

// Ellipse moving up/down
dx = 0;
dy = 2; // Positive for down, negative for up

``
