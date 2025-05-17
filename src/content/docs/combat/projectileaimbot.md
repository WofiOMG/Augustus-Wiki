# PROJECTILEAIMBOT
Automatically adjusts your aim when throwing or shooting projectiles (like bows, eggs, snowballs, potions, ender pearls, tridents, etc.) to hit moving targets. It rotates your view to improve accuracy while still allowing customizable legit-looking behavior.

## Modes:

**Independent:**
Aimbot runs separately from KillAura or rotation modules.

**Linear:**
Rotations follow a straight and constant path toward the target. Smooth but robotic.

**Curve:**
Rotations use curved easing, mimicking natural human aim more realistically.

## Rotation Speed Settings:

**MinYawSpeed / MaxYawSpeed:**
Minimum and maximum horizontal rotation speed (left/right) in degrees per tick.

**MinPitchSpeed / MaxPitchSpeed:**
Minimum and maximum vertical rotation speed (up/down) in degrees per tick.

**Acceleration Settings:**
MinYawAcceleration / MaxYawAcceleration:
Controls how quickly yaw rotation accelerates toward the target (makes it ramp up instead of instantly snapping).

**MinPitchAcceleration / MaxPitchAcceleration:**
Same as above, but for pitch (vertical).

If curve mode is enabled Randomizatiom: MinRandomStrength / MaxRandomStrength, RandomizeOnlyAtRotating wont be visible and will be replaced with the following settings:

**Interval:**
Time (in ticks) between curve updates.
Lower = faster curve changes.

**Amplitude:**
How far the aim moves off-center.
Higher = more visible wave motion.

**Frequency:**
How fast the wave moves.
Higher = quicker wiggles, lower = smoother aim.

**Randomization:**
MinRandomStrength / MaxRandomStrength:
Adds aim jitter to make your aim less perfect and more human-like.
Strength defines how much randomness is added to the final rotation.

**RandomizeOnlyAtRotating:**
If true, random jitter is only applied while turning, not when already aimed at target.

**BetterAcceleration:**
When true, uses a smoother and more realistic acceleration curve for aim transitions.

**Targeting Control:**
MaxTarget Look FovDiff:
Maximum field of view difference allowed between your current rotation and the target's location.
Prevents snapping to targets too far from your screen center.

**Combat:**
If true, activates only during combat or while using KillAura.

**Predict:**
Enables prediction of target movement (especially useful for long-range bow shots or moving targets).

**OnlyAtKillAura:**
When true, activates only when KillAura is enabled.

**OnlyKillAuraTarget:**
Limits aim adjustment to only the current KillAura target, ignoring other entities.

**AimRange:**
Maximum range (in blocks) at which aimbot will try to aim at a target.

**AssistAtRightClick:**
When true, aim assist activates only while holding right-click (for bows, potions, etc.).

**Targets:**
Defines what entities can be aimed at:
Player, Mob, Animal, Villager, ArmorStand, Invisible, Dead
Note: Not using AntiBot might cause the module to attack bots like shopkeepers.