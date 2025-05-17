# ANTIFIREBALL
The **AntiFireBall** module automatically targets and hits back fireballs, when they are within a specified range and under the right conditions. Use teams module to prevent hitting your teammates fireballs.


**MinYawSpeed**
The minimum yaw (horizontal rotation) speed in degrees per second when turning to face a fireball. Lower values make smoother but slower turns.

**MaxYawSpeed**
The maximum yaw speed when aiming. Higher values allow faster turns. If MinYawSpeed and MaxYawSpeed are different a random value between them will be taken.

**MinPitchSpeed**
The minimum pitch (vertical rotation) speed in degrees per second. Determines how fast the player looks up/down toward a fireball.

**MaxPitchSpeed**
The maximum pitch rotation speed. Together with MinPitchSpeed, controls aiming smoothness. If MinPitchSpeed and MaxPitchSpeed don't have the same value, a random value will be chosen every time.

**RotationMode**
Determines how the module calculates the angle to turn toward the fireball:
• Head – Aims based on the player’s head direction.
• BestHitVec – Calculates the best point on the fireball to hit.
• NearestHitVec – Aims at the closest possible hit point on the fireball.
-If BestHitVec or NearestHitVec is enabled, you have the following settings:

**HitBoxPercentageVertical**
Controls how high up and down the module will aim on the fireball.
1.0 = aims at the whole fireball height.
0.5 = aims near the middle.

**HitBoxPercentageHorizontal**
Controls how wide of the fireball's side the module can aim at.
1.0 = targets the entire width.
0.5 = focuses on the center

**AdvancedRoots**
When true, uses advanced math and smoothing for human-like rotation, reducing the chance of detection by anti-cheat systems.

**Interpolation**
Smooths the rotation between angles frame by-frame for visual consistency.

**RandomType**
Defines the algorithm used for adding randomness to your rotation, helping avoid anti-cheat detection:
• Random – Basic random.
• SecureRandom – Cryptographically secure randomness (slower but stealthier).
• Gaussian – Smooth curve-based randomness.
• Intave – Specifically mimics behavior acceptable to Intave anti-cheat.

**Randomize**
Controls what gets randomized:
• None – No randomization.
• Basic – Light variation.
• Doubled – Adds more variance.
• OnlyRotation – Only your aim is randomized.
• Advanced – Full randomization of movement and aim.

**RandomStrenght**
Controls how strong the randomization effect is.

**MoveFix**
When enabled, gives consistent player movement direction, even while the module changes your view angle. Prevents missteps or strange pathing.

**SilentMoveFix**
A variation of MoveFix that tries to hide the movement corrections. Options include:
• None – No silent move fix.
• Advanced – Applies hidden fixes without altering visible movement.

**SilentMoveFixIntave**
Specialized move fix logic to bypass the Intave anti-cheat system. Should be true if playing on such servers.

**NoRotate**
If true, disables actual view rotation while still interacting with fireballs, basically hits the fireball without turning the player which would flag most anti-cheats.

**PreAimRange**
Distance, at which the module will start tracking and aiming at fireballs.

**Delay**
Number of ticks to wait before reacting to a new fireball after the first one is hit. 1 second= 20 ticks.

**SlowDown**
When true, slows player movement slightly during aiming or while hitting a fireball, making it look more legit.

**TicksExsisted**
A condition to check how long the fireball entity has existed before the module will target it. Useful to avoid reacting to newly spawned fireballs close to you.

**NotWhileDigging**
If true, the module will not activate while you're mining or holding down left-click, preventing interruptions during block breaking.

<div style="border-left: 5px solid #3A87AD; background-color: #D9EDF7; padding: 15px; color: #31708F; font-family: Arial, sans-serif; border-radius: 6px; max-width: 700px; box-shadow: 0 2px 5px rgba(49,112,143,0.3);">
  <strong style="font-size: 18px; display: flex; align-items: center; margin-bottom: 10px;">
    ℹ️ Important Notes for AntiFireBall Module
  </strong>
  <ul style="font-size: 16px; line-height: 1.5; padding-left: 20px;">
    <li><strong>Use Teams Module:</strong> Prevents hitting teammates’ fireballs.</li>
    <li><strong>RotationMode:</strong> BestHitVec and NearestHitVec offer better accuracy but require tuning hitbox percentages.</li>
    <li><strong>Randomization Settings:</strong> Adjust <em>RandomType</em> and <em>Randomize</em> carefully to avoid anti-cheat detection.</li>
    <li><strong>MoveFix and SilentMoveFix:</strong> Enable these for smoother player movement while aiming.</li>
    <li><strong>SlowDown:</strong> Helps appear more legitimate but can reduce movement speed temporarily.</li>
    <li><strong>NotWhileDigging:</strong> Prevents interference during mining; enable if you frequently dig while using the module.</li>
  </ul>
</div>
