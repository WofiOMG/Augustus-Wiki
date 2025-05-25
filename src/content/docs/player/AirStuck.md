---
title: AirStuck
---
Freezes the player's position mid-air, often used for clutching or stopping movement temporarily.

### Mode
Controls how your rotation behaves while stuck:

- **NoRotate**: Rotation is locked **client-side** and not sent to the server. The server sees you as not turning.
- **CanRotate**: Rotation is **both client-side and server-side**. You can look around, and the server sees it too.
- **Intave**: Mimics **server-friendly** behavior tailored for Intave anti-cheat. Rotation may be partially sent to avoid detection.
- **NewNoRotate**: An improved version of **NoRotate**, still **client-side only**, possibly with smoother behavior.

### Sneak
Automatically sneaks while stuck, helpful for block placement or anti-cheat behavior.

### OnlyInAir
Only activates AirStuck when you are in the air — doesn’t trigger if you’re on the ground.
