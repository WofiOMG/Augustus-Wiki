---
title: BugUp
---
A module that exploits movement bugs to gain positional advantages by resetting you to your last on-ground position and manipulating movement packets.

### Mode  
Different methods for the bug exploit:

---
### Teleport  
Instantly moves the player to a target location.

---
### SetPosition  
Sets the player’s position directly without normal movement.

---
### OnGround  
Resets you to your last on-ground position.

---
### OnGroundSpoof  
Spoofs ground status to the server for various effects.

---
### Speed  
Increases movement speed during the bug.

---
### Jump  
Uses jumping to trigger the bug effect.

---
### Collision  
Manipulates collision detection for movement advantage.

---
### AirStuck  
Freezes player mid-air by exploiting movement packets.

---
### BlinkOutgoing  
Delays outgoing packets for teleport-like movement.

---
### BlinkBoth  
Delays both incoming and outgoing packets for advanced teleportation.

---
### AutoPlatform  
Automatically places blocks beneath the player to prevent falling.

---
### NCP  
A mode designed to bypass the NoCheatPlus anti-cheat.

---
### Mode:  
Teleport, SetPosition, OnGround, OnGroundSpoof, Speed, Jump, Collision, AirStuck, AutoPlatform

#### MaxFallDistanceWithoutBugUp  
Maximum fall distance allowed before BugUp activates.

#### BugUpOnlyIfFallingIntoVoid  
Only triggers BugUp when falling into the void.

#### MinBackFlagDist  
Minimum distance to trigger rollback or flag backing.

#### MaxBackFlagDist  
Maximum distance allowed for rollback or flag backing.

---
### Mode:  
BlinkOutgoing, BlinkBoth

#### MaxFallDistanceWithoutBugUp  
Maximum fall distance allowed before BugUp activates.

#### BugUpOnlyIfFallingIntoVoid  
Only triggers BugUp when falling into the void.

#### MinBlinkPackets  
Minimum number of packets delayed in Blink modes.

#### MaxBlinkPackets  
Maximum number of packets delayed in Blink modes.

---
### Mode:  
NCP

#### FallDistance  
Sets the fall distance threshold for activating BugUp in blocks.

#### MinBackFlagDist  
Minimum distance to trigger rollback or flag backing.

#### MaxBackFlagDist  
Maximum distance allowed for rollback or flag backing.