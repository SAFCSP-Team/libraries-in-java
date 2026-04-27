# Libraries Project

### Objective

This project focuses on understanding how to use libraries in Java.

### Problem

Draw a circle using Java libraries with user-provided size and position.

### Implementation

#### Define the `Circle` class:

- Inherit from the `Canvas` class.
- Add three attributes:
    - `int x, y`: to store the position of the circle.
    - `int radius`: to store the size of the circle.
- Create a constructor to initialize all attributes with the given parameters.
- Override `paint(Graphics g)` to:
    - Set the color to green.
    - Draw a filled circle using `x`, `y`, and `radius`.

#### In the `main` method: 
- Use a `Scanner` to prompt the user for:
    - The circle's position (`x`, `y`).
    - The circle's `radius`.
- Create a Frame object titled "Green Circle".
- Create an object of `Circle` using the user input.
- Set the canvas size to 300 x 300.
- Add the circle to the frame.
- Set the frame size to 300 x 300.
- Make the frame visible to display the circle.

### Output
If the user enters **x = 60**, **y = 60**, and **radius = 90**, the following window will appear:

<img width="347" height="325" alt="Screenshot 1447-11-10 at 12 47 43 PM" src="https://github.com/user-attachments/assets/4f590178-0204-476e-bc3e-026b3f13390d" />
