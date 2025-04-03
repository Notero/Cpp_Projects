# 🟩 SFML Collision Demo – Bouncing Shapes

## 🧾 Description
This project is a simple SFML-based animation demonstrating **basic collision detection and response** using `sf::FloatRect` boundaries. Two shapes—a `sf::CircleShape` and a `sf::RectangleShape`—bounce around within a window, reversing direction when they hit the window's edges.

## 🎮 Features
- 🟢 Bouncing **rectangle** (4x4 green block)
- 🔵 Bouncing **circle** (8px radius blue ball)
- 🧱 Custom edge-based collision using `sf::FloatRect`
- 🎨 Background `sf::VertexArray` line strip art

## 📐 Technical Details
- **SFML version:** 2.5+
- **Window size:** 1280×800
- **Shapes move** using velocity vectors (`sf::Vector2f`)
- **Edge collisions** are detected using `intersects()` against pre-defined invisible borders
- **Collision function** reverses the appropriate velocity component

## 📦 Files
- `main.cpp`: Core logic, shape updates, drawing, and window handling
- `Collision()` function: Takes a shape's bounds and current speed, then checks for intersections against window borders

## 🛠️ How to Build & Run
### 💻 Requirements
- SFML (2.5 or later)
- C++17 compatible compiler

### 🔧 Compilation (Windows example using g++)

    g++ main.cpp -o BounceApp -lsfml-graphics -lsfml-window -lsfml-system
    ./BounceApp

# 👤 Author
Akin Korkmaz
