# Pseudocode – Snake Game (Minimum 5 Functions)

This file contains the required pseudocode for core operations of the Snake Game.  
Each function is written in simple structured pseudocode format.

---

## 1. MoveSnake()
```
IF direction == UP:
    newHead.y = head.y - 1
ELSE IF direction == DOWN:
    newHead.y = head.y + 1
ELSE IF direction == LEFT:
    newHead.x = head.x - 1
ELSE IF direction == RIGHT:
    newHead.x = head.x + 1

INSERT newHead at the beginning of Linked List
REMOVE last node (tail) from Linked List
```

---

## 2. GrowSnake()
```
CREATE a new node
APPEND node at the tail of Linked List
```

---

## 3. GenerateFood()
```
REPEAT:
    x = random value in grid width
    y = random value in grid height
UNTIL grid[x][y] is empty

food.x = x
food.y = y
```

---

## 4. CheckCollision()
```
IF head.x < 0 OR head.x >= gridWidth:
    RETURN true   // Wall collision

IF head.y < 0 OR head.y >= gridHeight:
    RETURN true   // Wall collision

FOR each node in snake body (except head):
    IF head.x == node.x AND head.y == node.y:
        RETURN true   // Self collision

RETURN false
```

---

## 5. UpdateScore()
```
IF head.x == food.x AND head.y == food.y:
    score = score + 1
    CALL GrowSnake()
    CALL GenerateFood()
```
