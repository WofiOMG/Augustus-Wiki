# AUTOWALK
A movement module that automatically walks toward targets with advanced rotation control and pathfinding. This module can be combined with AutoPlay and KillAura to play sumo matches without user input. Useful for afk win streaks.

**MinYawSpeed / MaxYawSpeed**
Sets the range of yaw (horizontal) rotation speed.

**MinPitchSpeed / MaxPitchSpeed**
Sets the range of pitch (vertical) rotation speed.

## RandomType
Determines how randomness is applied to rotations:

**Random**
Basic Java Random, lightweight and fast.

**SecureRandom**
Cryptographically secure RNG, adds heavier variation.

**Gaussian**
Uses a normal distribution for more natural-looking randomness.

**Intave**
Mimics patterns designed to bypass Intave anti-cheat system.

## Randomize
Controls how much and what kind of randomness is added:

**None**
No randomization applied.

**Basic**
Adds standard random offsets.

**Doubled**
Doubles the effect of randomness.

**OnlyRotation**
Applies randomness only to rotation, not movement.

**RandomStrength**
Adjusts how strong/random the rotations are.

**AdvancedRots**
Enables smarter and more human-like rotations.

**Interpolation**
Smooths out rotation transitions between angles.

**PathFinding**
Allows walking around obstacles by calculating a path to the target.

**DebugLine**
Draws a line showing the current walking path.

**Distance**
Max distance to start walking toward a target.

**MaxSearch Time**
How long the module searches for a path before stopping.

**UpdateTicks**
Interval (in ticks) between path updates.

**Smooth**
Enables smoother, less robotic movement.

**KeepRotation**
Maintains the player's rotation while walking.

## MovementMode
Sets the logic used for movement:

**Rotation**
Movement is based on current rotation.

**Silent**
Moves without affecting visible rotation. Only server side rotations in first person view, similar to freelook.

**RotationUpdateTicks**
Tick interval for updating player rotation.

**Targets**
Defines what entities AutoWalk will follow: Player, Mob, Animal, Villager, ArmorStand, Invisible
Not using AntiBot correctly may cause the module to chase bots.

**OnlyWithKillAuraTarget**
Only activates AutoWalk when KillAura has a valid target.

**NoWalkDistanceToTarget**
Stops walking when within this distance to the target.

**Jump**
Allows jumping while walking. Use JumpFix in KillAura.

**StopWhileEating**
Disables walking while the player is eating.

**StopWhileSlowness**
Stops walking if affected by slowness.

**AdStrafeOnHit**
Enables automatic strafing after hitting a target.

**AdStrafeTime**
Duration of strafe after a hit.

**DelayAfterRespawn**
How long to wait after respawning before walking resumes.

