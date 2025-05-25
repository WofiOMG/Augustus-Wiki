---
title: Fucker
---
This module breaks spesific blocks automatically.

### MinYawSpeed:  
Minimum horizontal (yaw) rotation speed when turning toward the target block.

### MaxYawSpeed:  
Maximum yaw speed. Randomly picked between Min and Max for more human-like movement.

### MinPitchSpeed:  
Minimum vertical (pitch) rotation speed.

### MaxPitchSpeed:  
Maximum pitch speed. Affects how fast your view aims up/down toward beds or other blocks.

### RandomType: Random, SecureRandom, Gaussian, Intave  
Controls how randomness is generated:  
- **Random**: Basic Java randomness.  
- **SecureRandom**: Cryptographically secure, slower but less predictable.  
- **Gaussian**: Uses a bell-curve randomness for smoother, human-like aim.  
- **Intave**: Mimics a specific anti-cheat-safe pattern.

### Randomize: None, Basic, Doubled, OnlyRotation  
Adds extra randomness to aiming/motion:  
- **None**: No extra randomness.  
- **Basic**: Adds minor offset.  
- **Doubled**: Adds more aggressive/random variation.  
- **OnlyRotation**: Randomizes view rotation only, not movement.

### RandomStrength:  
How strong the aim randomness is. Higher = more offset and less predictable behavior.

### AdvancedRots:  
If true, enables more complex and legit rotation behavior.

### Interpolation:  
Smooths aim transitions between ticks. Helps avoid snapping.

### MoveFix:  
Prevents rotation from interfering with movement direction. This setting moves the player only server-side, not client-side.

### SilentMoveFix: None, Default, Advanced  
Fixes movement direction silently without affecting client view:  
- **None**: No fix.  
- **Default**: Basic yaw compensation.  
- **Advanced**: Smarter correction to avoid detection.

### SilentMoveFixIntave:  
Extra movement correction aimed at bypassing Intave anti-cheat.

### Block: Bed, Cake, Custom  
Chooses which type of block to target:  
- **Bed**: Standard bed destroyer.  
- **Cake**: For cake-based servers (rare).  
- **Custom**: Supports other block types via config.

### Action: Break, Click, Use  
Defines what action is done on the target block:  
- **Break**: Destroys the block.  
- **Click**: Right-clicks it one time.
- **Use**: Uses beds, eats cakes...

### Delay:  
Time (in ms) between each block interaction. Lower = faster action.

### AimRange:  
How close you need to be for the module to aim at a target block.

### Range:  
Maximum block interaction range.

### BreakOnlyFreeBeds:  
If true, only breaks beds that aren’t blocked by other blocks.

### ThroughWall:  
If true, allows breaking beds or targets through walls (ghost breaking).

### Instant:  
If enabled, breaks the target block instantly without visible mining.

### FriendMyBlock:  
Avoids breaking blocks placed by teammates or marked as friendly. .friend (name)

### BedBlink:  
Blinks (chokes packets until release) until released.

#### BedBlinkTime:
Delay before bed break packets are sent.