# Assignment 01 – OpenGL Cyan Window

## Course
CSE-358 Computer Graphics and Multimedia Lab

## Author
MD Raiyan

## Description
This program creates a cyan-colored window using OpenGL with GLFW and GLAD.
The window title displays the author's full name.
The application listens for keyboard input and closes the window when the
user presses the **R** key.

## Tools & Libraries Used
- C++
- OpenGL 3.3 Core Profile
- GLFW
- GLAD

## Window Details
- Window Width: 800 pixels
- Window Height: 600 pixels
- Window Title: MD RAIYAN
- Background Color: Cyan (RGB: 0.0, 1.0, 1.0)

## Keyboard Control
- Press **R** → Close the window

## How the Program Works
1. Initializes GLFW and configures OpenGL version 3.3.
2. Creates a window with a cyan background.
3. Loads OpenGL function pointers using GLAD.
4. Continuously renders the window inside a loop.
5. Listens for keyboard input.
6. Terminates the program when the **R** key is pressed.

## How to Run
1. Make sure GLFW and GLAD are properly installed.
2. Compile the program using a C++ compiler.

Example (Linux / MinGW):
```bash
g++ main.cpp -lglfw -lopengl32 -o Assignment01
