# Operation Flow Explanation – Snake Game

Below are three operations explained in detail according to the required format.

---

## 1. Move Snake  
**What the operation does:**  
Moves the snake one step in the current direction.

**Data Structure Used:**  
Linked List (each node = snake part)

**Why this DS is suitable:**  
Fast insertion at head and deletion at tail makes movement efficient.

**How the user interacts:**  
User presses arrow keys; direction updates; Linked List head moves accordingly.

---

## 2. Generate Food  
**What the operation does:**  
Creates food at a random position on the game grid.

**Data Structure Used:**  
Struct {int x, y} + 2D grid

**Why this DS is suitable:**  
Struct stores coordinates neatly; grid helps ensure food does not spawn on snake body.

**How the user interacts:**  
User visually sees new food appearing on screen.

---

## 3. Collision Detection  
**What the operation does:**  
Checks if snake hits a wall or its own body.

**Data Structure Used:**  
2D Array (grid)

**Why this DS is suitable:**  
Grid allows constant-time boundary checking and detecting snake body collisions.

**How the user interacts:**  
If collision happens, game stops and “Game Over” message appears.
