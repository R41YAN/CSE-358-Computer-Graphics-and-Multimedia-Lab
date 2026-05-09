# ⭐ Assignment 05: Rotating & Scaling Rectangle Using OpenGL

## 📋 Description
This OpenGL application renders **one rectangle** (composed of two triangles) that **rotates**, **scales**, and **changes color** dynamically over time using shader uniforms and GLM transformation matrices. The program demonstrates the use of **Modern OpenGL (Core Profile)** concepts such as vertex buffers, vertex arrays, shader programs, uniform variables, and matrix transformations. Keyboard input is also implemented to close the window.

---

## ✅ Requirements Fulfilled
- Rectangle rendered using two triangles with `glDrawArrays(GL_TRIANGLES)` (no EBO)
- Rectangle rotates continuously around the Z-axis
- Rectangle scales in and out smoothly over time
- Rectangle color pulses dynamically between **white and red**
- GLM transformation matrix applied (rotation + scale combined)
- Keyboard interaction implemented using GLFW
- Vertex Array Object (VAO) and Vertex Buffer Object (VBO) used
- Modern OpenGL **Core Profile (3.3)** followed
- Proper code structure, formatting, and comments
- Original work implemented and tested locally
- README documentation included

---

## 🔧 Program Features
- **Graphics API:** OpenGL 3.3 Core Profile
- **Window Management:** GLFW
- **Function Loader:** GLAD
- **Math Library:** GLM (matrix transforms)
- **Primitive Used:** Two Triangles (forming a Rectangle)

---

## 🪟 Window Properties
- **Resolution:** 800 × 600 pixels
- **Background Color:** Black `(0.0, 0.0, 0.0)`
- **Window Title:** 0432320005101101

---

## 🎨 Rendering Details
- One rectangle rendered at the center of the window
- Rectangle built from **6 vertices** forming 2 triangles (no Element Buffer Object)
- Rendering performed using:
  - Vertex Buffer Object (VBO)
  - Vertex Array Object (VAO)
- Fragment shader uses a **uniform variable** to control color
- Vertex shader uses a **uniform mat4 transform** for rotation and scale

### 🔄 Rotation
- Rotates around the **Z-axis** (spins in the XY plane)
- Speed: `glfwGetTime() * 0.5`

### 📐 Scale Pulse
- Scale driven by `sin(glfwGetTime() * 0.5)`
- Rectangle scales between **0.5×** and **1.5×** smoothly

### 🎨 Color Pulse
- Red channel stays fixed at `1.0`
- Green and Blue channels driven by `sin(time * 0.5)`
- Smoothly transitions between:
  - **White** `(1.0, 1.0, 1.0)`
  - **Red** `(1.0, 0.0, 0.0)`

---

## ⌨️ Keyboard Interaction
- Keyboard input handled using GLFW

| Key | Action |
|-----|--------|
| **R** | Closes the window |

---

## 🧪 Technologies Used
- **C++**
- **OpenGL**
- **GLFW**
- **GLAD**
- **GLM**
- **stb_image**

---

## 📸 Output Screenshot
![Rectangle Output](Output.png)

---

## 🧑‍🎓 Author
**Md. Raiyan**
ID – 0432320005101101

---

## 📝 Notes
- The rectangle is rendered using the Modern OpenGL pipeline
- GLM `glm::rotate` and `glm::scale` are combined into a single transform matrix
- All animations (rotation, scale, color) run at **0.5× speed** for a smoother look
- No deprecated OpenGL functions are used
- Project is intended for **academic and learning purposes**

---
