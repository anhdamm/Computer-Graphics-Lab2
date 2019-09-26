# Anh Dam - Lab 2 

## This lab is created to implement Bresenham's midpoint line scan conversion algorithm and Bresenham's midpoint circle scan conversion algorithm. 

### Requirements:
- Create a GLUT window
- Create a user-defined init function that clears the viewport to black
- Create a keyboard callback function that allows the user to type "q" to exit the application
- Create reshape callback function when the window is changed
- Answer the given questions.

### Midline Algorithm explanation:
- Using the line function, (x,y) = ax + by + c = 0 and 
- y = (dy/dx)x + B then (by subtract y from both sides/mult. by dx)
- F(x,y) = dy(x) - dx(y) + dx(B) = 0 where a = dy, b = -dx, c = dx(B)
- For points on the line F(x,y) = 0, F is positive for points below the line and negative for points above the line.

## Midcircle Algorithm explaination:
- Given a circle centered at (0,0) and radius r and a point p(x,y)
- F(p) = x2 + y2 – r2
- If F(p)<0, the point is inside the circle
- F(p)=0, the point is on the perimeter
- F(p)>0, the point is outside the circle
