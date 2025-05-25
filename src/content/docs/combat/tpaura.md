---
title: TPAuara
---
A powerful combat module that teleports you to targets (or simulates teleportation via packets), attacks them, then returns to your original position — allowing long-range kills while appearing legit or bypassing detection.

### MaxDistance:
Controls how far away TPAura will search for targets in blocks/meters.

### MaxTeleportDistance:
The maximum distance you're allowed to teleport to hit a target. Limits how far it simulates or sends attack packets.

### AttacksPerSecond:
Sets how many times per second TPAura will strike a target. Controls attack speed.

### NoSwing:
If enabled, disables arm-swing animation when attacking.

### Fly:
If enabled, allows TPAura to teleport through the air to hit airborne targets or avoid terrain collisions.

### Target:
Specifies what entities can be attacked:  
Player, Mob, Animal, Villager, Invisible, Dead  
*Note: Not using antibot might cause TPAura to attack bots like shopkeepers.*

### MaxTargets:
Maximum number of targets TPAura will attack in one cycle.

### MinHurtTime:
Minimum hurtTime (in ticks) the target must have before attacking again (prevents hitting during invincibility frames). Lower = faster re-hits.

### DebugLines:
Shows visual lines between you and your targets while attacking (useful for testing or visual feedback).

### Legit:
When enabled, makes teleportation more realistic or subtle (delays, slower pathing, obeying anti-cheat boundaries). May sacrifice speed for stealth.
