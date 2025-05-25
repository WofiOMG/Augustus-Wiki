---
title: TimeRange
---
TimerRange manipulates the game’s internal timer speed to speed up or slow down actions like attacks, movement, or block placing. It controls how fast game ticks advance, helping with faster clicks or actions while trying to remain undetected by anti-cheat systems.

### Delay  
The base delay in milliseconds before the timer effect starts.

### TimerTicksForward  
The number of game ticks the timer moves forward (speeds up) when active.

### Tolerance  
The amount of allowed variation in timing to avoid detection or glitches.

### BalanceCheck  
Enables balancing checks to keep the timer changes subtle and fair.

### MinAdditionalStop  
The minimum extra random pause added after the delay to make timing less predictable.

### MaxAdditionalStop  
The maximum extra random pause added after the delay for variability.

### OnlyOnGround  
If enabled, the timer only works when the player is on the ground (not mid-air).

### Dynamic  
Allows the timer to adjust dynamically based on in-game conditions.

### OnlyKillAura  
The timer only activates when KillAura (automatic attacking) is enabled.

### ClickCheck  
Synchronizes timer changes with player clicks to maintain consistency.

### ForbiddenSneak  
Disables the timer while sneaking to avoid detection or glitches.

### FixMode  
Applies specific fixes or optimizations to improve timer stability or avoid anti-cheat flags.

### None  
No fix mode.

### Fix1  
Usually targets basic timing inconsistencies or synchronization problems, smoothing out timer speed changes to avoid sudden jumps that can trigger anti-cheats.

### Fix2  
Typically a more advanced or aggressive fix that may include additional corrections or tweaks for specific edge cases where Fix1 isn’t enough.