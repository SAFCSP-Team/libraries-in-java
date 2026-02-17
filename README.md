# Libraries Project


### Objective

The main goal of this project is to learn how to use drawing libraries in Java (Swing and AWT) and how to retrieve user input.

### Problem

Draw the circle using Java’s libraries with user-provided size and color. 

### Implementation

#### 1. **Define a `Circle` Class**

- **Fields:**
    - `int x, y`: Coordinates of the circle's center.
    - `int radius`: The radius of the circle.
    - `Color color`: The color of the circle.

- **Constructors:**
    - `public Circle(int x, int y, int radius, Color color)` to initializes all fields with the given parameters.
    - `public Circle(int radius, Color color)` to set `x` and `y` to default ( e.g., center of window), and uses the given `radius` and `color`.

- **Method:**
    - `public void draw(Graphics g)` to draw the circle by setting the graphics color and drawing the filled circle.

#### 2. **Define a `CirclePanel` Class**

- **Inherit from** `JPanel`.
- **Field:**
    - `Circle circle`: to store the circle to be drawn.
- **Constructor:**
    - `public CirclePanel(Circle circle)` To store the passed-in `Circle` object, and sets the panel's preferred size.
- **Method:**
    - Override `protected void paintComponent(Graphics g)`: don't forget to call the `super.paintComponent(g)` first, then draw the circle.

#### 3. In the `main` Method of the `Main` Class

- Use a `Scanner` to prompt the user for:
    - The circle's **radius**.
    - The circle's **color**.
- Use a **switch statement** (or if-else) to map the color name to a `Color` object. Provide a default value (e.g., gray) for invalid input.
- **Create the `Circle` object** using the user's choices.
- **Create the window using Swing:**
    - Create a `JFrame`.
    - Add a new `CirclePanel` with the `Circle` you created. 
    - Size the frame to its panel.
    - Call `setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE)` and `setVisible(true)` to display the window centered on the screen.
