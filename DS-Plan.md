# Data Structure Planning Table – Snake Game

This table includes at least five operations from our Snake Game and the data structures used for each.  
Each group member contributed one operation.

---

## 1. Move Snake  
**Member:** Muhammad Waleed Iqbal (184)  
**Operation:** Move the snake forward  
**Data Structure Used:** Linked List  
**Reason:** Snake grows and shrinks dynamically. Linked List supports fast insertion at the head and deletion at the tail.  
**How it works:** New head node is added; tail node is removed.

---

## 2. Grow Snake  
**Member:** Haseeb Ali (233)  
**Operation:** Increase snake length after eating food  
**Data Structure Used:** Linked List  
**Reason:** Allows dynamic addition of a new node at the tail without resizing.  
**How it works:** A new node is appended at the tail.

---

## 3. Food Generation  
**Member:** Abu Bakar Saeed (225)  
**Operation:** Generate new food at random location  
**Data Structure Used:** Struct (x, y) + 2D Array Grid  
**Reason:** Coordinates are stored easily in a struct; grid helps check empty space.  
**How it works:** Random x,y stored in struct, validated using grid array.

---

## 4. Collision Detection  
**Member:** Ahad Mehmood (223)  
**Operation:** Check collision with wall or self  
**Data Structure Used:** 2D Array (Grid)  
**Reason:** Grid allows constant-time check of boundaries and snake-body presence.  
**How it works:** If head position touches wall or matches any grid cell containing snake → Game Over.

---

## 5. Score Update  
**Member:** Group  
**Operation:** Increase score when food is eaten  
**Data Structure Used:** Integer Variable  
**Reason:** Simple counter updated constantly.  
**How it works:** score++ whenever snake eats food.
