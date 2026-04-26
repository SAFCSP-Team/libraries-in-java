# Libraries Project

### Objective

This project’s main focus is on understanding how to use libraries in Java.

### Problem

Draw the circle using Java’s libraries with user-provided size and position. 

### Implementation
#### 1. **Define a `Circle` Class** that : 
- **Inherit from** `Canvas` class.
- **Fields:**
    - `int x, y`: Coordinates of the circle's center.
    - `int radius`: The radius of the circle.

- **Constructors:**
    - `public Circle(int x, int y, int radius)` to initializes all fields with the given parameters.

- **Method:**
    - Overrides `public void paint(Graphics g)` to set the color to green and draw a filled circle based on the given coordinates and radius.
#### 2. In the `main` method 
- Use a `Scanner` to prompt the user for:
    - The circle's **radius**.
    - The circle's position **x**, **y**.
- **Create a Frame object** titled "Drawing Example".
- **Create an object of DrawingExample** using the user input.
- **Set the canvas size** to 300 x 300.
- **Add the canvas to the frame**.
- Set the frame size and make it visible to display the drawn circle.
