---
title: KeepSprint
---
Prevents the game from stopping your sprint when you attack or perform certain actions.
Vanilla behavior: When you hit an entity, Minecraft cancels your sprint. This module keeps you sprinting even after attacking.

### MoveSlowdownOnGround  
Prevents the slowdown effect when moving on the ground and using items (e.g., blocking with sword, eating). Helps maintain sprint.

### SprintOnGround  
Keeps sprinting enabled while on the ground — even when attacking. Overrides the vanilla sprint reset on hit.

### MoveSlowdownInAir  
Prevents movement slowdown when hitting enemies in the air.

### SprintOnGroundInAir  
When enabled, forces sprinting both on ground and in the air.

### Smart  
Uses smarter conditions to avoid triggering anti-cheat detections — for example, disabling KeepSprint when suspicious item use or invalid movement is detected.

### KeepSprint Module Overview

- **KeepSprint Module**
  - 🚫 *Prevents:*  
    - Vanilla: Stops sprint on hit  
    - MoveSlowdownOnGround: No slowdown on ground  
    - MoveSlowdownInAir: No slowdown in air  
  - ✅ *Maintains:*  
    - SprintOnGround: Sprint while attacking  
  - 🔥 *Forces:*  
    - SprintOnGroundInAir: Sprint on ground & air  
  - 🧠 *Smart mode:*  
    - Avoid anti-cheat detection
