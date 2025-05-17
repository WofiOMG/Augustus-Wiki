# KEEPSPRINT
Prevents the game from stopping your sprint when you attack or perform certain actions.
Vanilla behavior: When you hit an entity, Minecraft cancels your sprint. This module keeps you sprinting even after attacking.

**MoveSlowdownOnGround:**
Prevents the slowdown effect when moving on the ground and using items (e.g., blocking with sword, eating). Helps maintain sprint.

**SprintOnGround:**
Keeps sprinting enabled while on the ground — even when attacking. Overrides the vanilla sprint reset on hit.

**MoveSlowdownInAir:**
Prevents movement slowdown when hitting enemys in air.

**SprintOnGroundInAir:**
When enabled, forces sprinting both on ground and in the air. 

**Smart:**
Uses smarter conditions to avoid triggering anti-cheat detections — for example, disabling KeepSprint when suspicious item use or invalid movement is detected.

````mermaid
graph LR
A[KeepSprint Module] -->|prevents| B[Vanilla: Stops sprint on hit]
A -->|prevents| C[MoveSlowdownOnGround: No slowdown on ground]
A -->|maintains| D[SprintOnGround: Sprint while attacking]
A -->|prevents| E[MoveSlowdownInAir: No slowdown in air]
A -->|forces| F[SprintOnGroundInAir: Sprint on ground & air]
A -->|smart mode| G[Smart: Avoid anti-cheat detection]

style A fill:#bbdntstroke:#1976d2,stroke-width:3px
style B fill:#e3fv2fd,stroke:#64b5f6,stroke-width:2px
style C fill:#c8ev6c9,stroke:#388e3c,stroke-width:2px
style D fill:#c5ceae9,stroke:#303f9f,stroke-width:2px
style E fill:#ffwf9c4,stroke:#fbc02d,stroke-width:2px
style F fill:#ffcacbc,stroke:#d84315,stroke-width:2px
style G fill:#d1cx4e9,stroke:#512da8,stroke-width:2px

linkStyle 0,1,2,3,4,5 stroke:#333,stroke-width:4px,stroke-linecap:round
````