# BOWAIMBOT
BowAimbot automatically aims your bow at targets to improve accuracy and hit rate. It smoothly adjusts your aim and can auto-shoot when locked on, helping you land shots on enemies or other entities without manual aiming.

## Mode: New, Old

**Old:** 
Uses a simpler, more direct aiming method.

**New:** 
Uses a smoother, more advanced aiming method for more natural and harder-to-detect aiming.

## Rotations Mode:
Controls how your aim rotates to track targets.

**Independent:**
 Yaw and pitch rotate independently.

**Linear:**
 Smooth linear rotation towards target.

**Curve**
 Adds wave-like, sine curve motion to the rotation for more human-like movement.

**MinYawSpeed / MaxYawSpeed:**
Minimum and maximum speed for horizontal rotation (left-right aiming).

**MinPitchSpeed / MaxPitchSpeed:**
Minimum and maximum speed for vertical rotation (up-down aiming).

**MinYawAcceleration / MaxYawAcceleration:**
Minimum and maximum acceleration for horizontal rotation speed, controlling how fast the speed changes.

**MinPitchAcceleration / MaxPitchAcceleration:**
Minimum and maximum acceleration for vertical rotation speed.

### If you use Curve rotation mode you will have Interval, Amplitude and Frequency, if you use Independent or Linear mode you will have Min/MaxRandomStrenght and RandomizeOnlyAtRotation.

**Interval:**
Time between rotation updates in ticks (how often the aim adjusts).

**Amplitude:**
Controls the maximum strength of the wave motion in Curve mode (how much your aim wiggles).

**Frequency:**
Controls how fast the wave oscillates in Curve mode (speed of the wiggle).

**MinRandomStrength / MaxRandomStrength:**
Minimum and maximum randomness added to aim for more natural movement.

**RandomizeOnlyAtRotation:**
Whether to apply randomness only when the aim is rotating.

**BetterAcceleration:**
Enhances acceleration handling for smoother and more natural aiming.

**Fov (Field of View):**
Angle in degrees around your crosshair within which targets will be aimed at. Higher values mean more targets can be aimed at around you.

**SilentMoveFix:**
Fixes issues when moving silently while aiming. Options: None (no fix), Default (basic fix), Advanced (best fix).

**MoveFixIntave:**
Enables movement fixes tailored for Intave servers, improving aim stability.

**AutoShoot:**
Automatically fires the bow when your aim is locked on a target.

**No Horizontal Bruteforce:**
Prevents unnatural fast horizontal spinning to keep aiming looking legit.

### Entities:
Types of entities the aimbot targets: Players, Mobs, Animals, Invisible entities.
Note: Not using AntiBot might cause the module to attack bots like shopkeepers.

```mermaid
graph TD
  A[🎯 AutoShoot enabled] --> B[⚠️ May look suspicious without smooth aim]
  A --> C[✅ Combine with Curve or Linear rotation]
  D[🧠 No AntiBot] --> E[⚠️ Might aim at fake entities or NPCs]
  F[🎥 High FOV] --> G[⚠️ Can cause odd rotations on targets behind you]
  
  style A fill:#e0f7fa,stroke:#4dd0e1,stroke-width:2px
  style B fill:#ffe6e6,stroke:#ff8a80,stroke-width:2px
  style C fill:#e8f5e9,stroke:#81c784,stroke-width:2px
  style D fill:#f3e5f5,stroke:#ba68c
