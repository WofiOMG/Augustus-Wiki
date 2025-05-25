---
title: Velocity
---
Reduces or cancels knockback and other motion effects caused by attacks, explosions, or other sources to help you maintain control and avoid being pushed around.

## Modes:

---
### Intave13:
Cancels or reduces knockback by manipulating movement packets specifically made for Intave anti-cheat.

---
### Basic:
Simply reduces knockback by scaling down the player’s velocity after being hit.

---
### Grim-1.17:
Targets knockback patterns from Minecraft 1.17, adjusting motion accordingly to reduce KB.

---
### CustomMotion:
Applies a user-customizable velocity adjustment, allowing precise control over KB reduction.

---
### Reverse:
Inverts or reverses knockback motion to counteract the push effect.

---
### Legit:
Reduces knockback in a way that mimics normal player behavior to avoid detection.

---
### Karhu:
Uses a specialized algorithm to reduce knockback commonly effective on servers using Karhu anti-cheat.

---
### PushGround:
Focuses on reducing knockback while the player is on the ground, ignoring air knockback.

---
### Intave/PolarFlag:
Combines techniques to bypass Intave and Polar anti-cheats by managing velocity packets and motion.

---
### Spoof:
Spoofs player position or velocity packets to confuse server-side knockback calculations.

---
### Safewalk:
Integrates knockback reduction with safe movement, preventing knockback-related slips or falls.

---
### OldMinemen:
Tailored to reduce knockback on servers using older Minemen anti-cheat versions.

---
### Hypixeltest:
Adjusts velocity to counter knockback on Hypixel’s specific anti-cheat system.

---
### Intave:
A variant focused solely on Intave anti-cheat knockback mechanics.

---
### BoundingBlox:
Uses bounding box adjustments to mitigate knockback effects.

---
### PolarBlock:
Reduces knockback by blocking or canceling specific polar motion packets.

---
### Push:
General knockback push reduction by canceling or modifying push vectors.

---
### PacketCanceling:
#### CancelType:
Tells the module when to cancel the packet:

#### None:
Never cancel.

#### OnlyOnGround:
 Cancel only when you're standing on the ground.

#### OnlyInAir:
Cancel only when in the air.

### Always:
Always cancel the packets.

#### 500PacketKeepAlive:
**Purpose: **
Keeps your connection active by confirming you're still online.

#### Canceling:
 Simulates lag or desync. Often used to make anti-cheat systems ignore knockback or movement inconsistencies.

#### S32PacketConfirmTransaction
Purpose:
 Sent when interacting with your inventory (clicking, moving items).

#### Canceling: 
Can hide or delay inventory actions from the server, which helps spoof movement or avoid detection when performing fast or illegal inventory actions.

#### S48PacketResourcePackSend
Sent when the server attempts to make you download and apply a resource pack.

#### Canceling:
 Prevents forced resource pack downloads. Sometimes used to interfere with specific server-side triggers that rely on this packet. Not directly related to combat but can help prevent detection or forced visuals.

#### PacketCount:
How many times this packet should be canceled. Optional — used for fine control (e.g., only cancel 6 times, not infinitely).

### Settings for the specified modes: Intave13, Grim-1.17, Karhu, Intave/PolarFlag, Spoof, SafeWalk, OldMinemen, HypixelTest, PolarBlock

Intave/PolarFlag Has an aditional setting called Polar:true/false. Have it at true if the server users polar anti cheat and false if it uses other anti-cheats such as Intave.

#### NotWhileSPressed:
Disable velocity cancel when sprint key is pressed.

#### NotWhileLongJump:
Disable velocity cancel during long jump.

#### IgnoreFire:
Ignore fire damage knockback effects.

#### CancelDamageSoundsFromOtherPlayers:
Prevents damage sound packets from other players for less client lag or distraction.

#### PacketCanceling:
Enables canceling certain packets to reduce knockback.

PacketsToCancel:
S00PacketKeepAlive
S32PacketConfirmTransaction
S48PacketResourcePackSend

---
### Mode: Basic

#### VelocityPacket

#### XZVelocityInAir:
Controls horizontal velocity when in the air.

#### VelocityInAir:
Controls overall velocity when in the air.

#### CancleInAir
Cancels knockback while airborne.

#### XZVelocityOnGround:
Controls horizontal velocity when on the ground.

#### VelocityOnGround:
Controls overall velocity when on the ground.

#### CancelGround:
Cancels knockback while on the ground.

#### ExplosionPacket

#### Explosion:
Enables explosion knockback handling.

#### XZVelocityInAirExplosion:
Controls horizontal velocity in air from explosions.

#### VelocityInAirExplosion:
Controls overall velocity in air from explosions.

#### CancelAirExplosion:
Cancels air knockback caused by explosions.

#### XZVelocityOnGroundExplosion:
Controls horizontal velocity on ground from explosions.

#### VelocityOnGroundExplosion:
Controls overall velocity on ground from explosions.

#### CancelGroundExplosion:
Cancels ground knockback caused by explosions.

#### IntervalOptions

#### NotWhileSPressed:
Does not cancel velocity if sprint key is pressed.

#### NotWhileLongJump:
Does not cancel velocity during long jumps.

#### Lag:
Delay or lag adjustment for velocity canceling.

#### IgnoreFire:
Igores knockback caused by fire damage.

#### CancelDamageSoundsFromOtherPlayers:
Cancels damage sound packets from other players to reduce lag or distractions.

#### PacketCanceling:

#### PacketsToCancel:
S00PacketKeepAlive  
S32PacketConfirmTransaction  
S48PacketResourcePackSend

### CustomMotion

#### XZMotionInAir:
Controls horizontal motion reduction while in the air.

#### XZMotionOnGround:
Controls horizontal motion reduction while on the ground.

#### NotWhileSPressed:
Disables velocity canceling if the sprint key is pressed.

#### NotWhileLongJump:
Disables velocity canceling during long jumps.

#### Lag:
Sets lag or delay for velocity adjustments.

#### IgnoreFire:
Ignores velocity changes caused by fire damage.

#### CancelDamageSoundsFromOtherPlayers:
Cancels damage sound packets from other players to reduce lag or distractions.

### PacketCanceling:

#### PacketsToCancel:
S00PacketKeepAlive  
S32PacketConfirmTransaction  
S48PacketResourcePackSend

### Mode: Reverse

#### ReverseStart:
Activates reverse velocity movement at the start of a hit (pushes player opposite to knockback).

#### ReverseStrafe:
Controls strafing movement direction reversal to counter knockback, value 1 means enabled.

#### XZ-Velocity Strength:
Strength of horizontal (X and Z axis) velocity reversal to reduce knockback.

#### Y-Velocity Strength:
Strength of vertical (Y axis) velocity reversal to reduce knockback.

#### NotWhileSPressed:
Disables reverse velocity if sprint key is pressed.

#### NotWhileLongJump:
Disables reverse velocity during long jumps.

#### Lag:
Delay or lag setting for velocity manipulation.

#### IgnoreFire:
Ignores velocity effects caused by fire damage.

#### CancelDamageSoundsFromOtherPlayers:
Cancels damage sound packets from others to reduce distractions.

#### PacketCanceling:
#### PacketsToCancel:
S00PacketKeepAlive  
S32PacketConfirmTransaction  
S48PacketResourcePackSend

---
### Mode: Legit

#### JumpInInv:
Allows velocity jump logic to work even while inventory is open.

#### JumpDelay Mode:

#### Chance:
Uses random chance to decide if a jump will happen when hit.

#### JumpChance:
A percentage (e.g., 100) controlling the likelihood of a jump being triggered when eligible.

#### IntervalDelay:
Uses timing rules to decide if and when to jump, possibly with realistic delay patterns.

#### MinJumpInterval / MaxJumpInterval:
Range of ticks between jumps. Controls how often the player jumps to reduce velocity.

#### NotInARow:
Prevents repeating velocity jumps too frequently in succession.

#### Outliers:
Enables occasional irregular jump intervals to appear more legit.

#### MinJumpIntervalOutlierValue / MaxJumpIntervalOutlierValue:
Defines outlier timing range when Outliers is enabled.

#### MinOutlierDelay / MaxOutlierDelay:
Time between outlier events.

#### Normal Distribution:
Distributes jump timing using bell-curve-like randomness for more natural intervals.

#### Sigma:
Controls variance of the normal distribution.

#### Center:
Mean value around which the distribution is centered.

#### MinTickDelayBetweenJumps / MaxTickDelayBetweenJumps:
Delay between jump actions when triggered.

#### CheckFallDamage:
Only applies jumps if fall damage would be avoided or mitigated.

#### FallDistance / FallDistanceBufferSize:
Threshold for how much falling triggers a velocity jump.

#### NotWhileSpeed / NotWhileJumpBoost:
Disables jumping when player has speed/jump boost.

#### NotWhileSPressed / NotWhileLongJump:
Disables if sprint or long jump is active.

#### Lag:
Optional delay or pause under lag conditions.

#### IgnoreFire:
Disables the effect when on fire.

#### CancelDamageSoundsFromOtherPlayers:
Hides other players’ damage sounds.

#### PacketCanceling:
Cancels specific packets:

S00PacketKeepAlive  
S32PacketConfirmTransaction  
S48PacketResourcePackSend

---

### Mode: PushGround

#### StartHurtTime:
The hurt time (in ticks) when the pushground effect starts working. Lower values apply reduction immediately after getting hit.

#### EndHurtTime:
The hurt time tick when the pushground effect stops. Higher values extend the protection.

#### NotWhileSPressed:
Disables pushground if you're holding the backward (S) key.

#### NotWhileLongJump:
Disables pushground during long jump modules (helps with bypass and legit look).  
(true = active only outside long jumps)

#### Lag:
Optional delay (in ticks) to simulate network lag behavior. Often kept at 0 for responsiveness.

#### IgnoreFire:
If true, disables effects while on fire.

#### CancelDamageSoundsFromOtherPlayers:
Prevents playing the hurt sound from others. Mainly aesthetic, can reduce attention in replays or logs.

#### Packet Canceling:
These help reduce knockback and simulate lag by delaying or cancelling important communication with the server.

#### 500PacketKeepAlive
- **CancelType:** None / OnlyOnGround / OnlyInAir / Always  
- **PacketCount:** 6  
Cancels keep-alive packets to simulate disconnection or delay knockback handling.

#### S32PacketConfirmTransaction
- **CancelType:** Same as above  
- **PacketCount:** 1  
Cancels or delays inventory transactions to prevent detection of fast switches or spoofed movements.

#### S48PacketResourcePackSend
- **CancelType:** Same as above  
- **PacketCount:** 6  
Blocks forced resource pack downloads—helps avoid certain visual-based server checks.

---

### Mode: Intave

#### XZOnHit:
How much horizontal velocity (knockback) is allowed when hit. 0.80 will make you take 80% of the KB so 20% is reduced.

#### XZOnHitSprint:
Adjusts horizontal velocity when sprinting.

#### IntaveSmart:
Enables logic to automatically adapt to different anti-cheat behavior (bypass assist).

#### IntaveBoost:
Simulates movement boost to appear legit while reducing KB.

#### IntaveBoostDelay:
Delay (in ms) between boost attempts to avoid detection.

#### IntaveBoostOnGroundTicks:
How many ticks you must be on ground before boost can apply.

#### XZVelocity:
Manual control of horizontal velocity after hit (negative values = reverse motion).

#### YVelocity:
Vertical velocity control (jump effect after hit).

#### SneakInAir:
Sneaks while airborne—used to reduce KB and spoof fall status.

#### Water:
Enables special KB logic in water.

#### WaterInterval:
Interval for applying water logic.

#### Cobweb:
Applies anti-KB logic in cobwebs.

#### Ladder:
Enables velocity bypass while on ladders.

#### LadderXZOnly:
Limits ladder logic to horizontal direction only.

#### Jump:
Enables micro-jumping or hop-based bypassing after hit.

#### JumpInInv:
Performs jumps while inventory is open to help reduce motion lag abuse.

#### JumpDelay Mode:
- **Delay:** waits a fixed time between jumps  
- **Tick:** jumps based on tick intervals  
- **Chance:** random chance per tick

#### MinJumpDelay / MaxJumpDelay:
Delay range between allowed jumps (used in delay/tick modes).

#### Fall Check:

#### CheckFallDamage:
Avoids jumping or bypassing if it would cause fall damage.

#### FallDistance:
Max distance before it stops jumping to avoid taking damage.

#### FallDistanceBufferSize:
Buffers values to smooth transitions.

#### Conditional Limits:
- **NotWhileSpeed / NotWhileJumpBoost / NotWhileSPressed / NotWhileLongJump:**  
Disables KB reduction if any of these modules or keys are active, to keep movement legit-looking.

#### Lag:
Optional lag simulation delay (0 ticks/none).

#### IgnoreFire:
Disable effects if you're on fire.

#### CancelDamageSoundsFromOtherPlayers:
Mutes other players’ hit sounds (cosmetic or desync effect).

#### Packet Canceling:
Used to spoof lag, delay server updates, or bypass checks.

#### S00PacketKeepAlive
- **CancelType:** None / OnlyOnGround / OnlyInAir / Always  
- **PacketCount:** 6

#### S32PacketConfirmTransaction
- **CancelType:** None / OnlyOnGround / OnlyInAir / Always  
- **PacketCount:** 1

#### S48PacketResourcePackSend
- **CancelType:** None / OnlyOnGround / OnlyInAir / Always  
- **PacketCount:** Number of packets to cancel.


---

### Mode: BoundingBox

#### StartHurtTime:
Defines the time window (in ticks) after taking damage when the velocity manipulation is active.

#### NotWhileSPressed:
Disables the effect if you're holding the S (backward) key.

#### NotWhileLongJump:
Disables the effect while LongJump module is active.

#### Lag:
Adds an artificial delay before applying the velocity logic (measured in ticks).

#### IgnoreFire:
Ignores hurt events caused by fire (so the mode won’t activate from fire ticks).

#### CancelDamageSoundsFromOtherPlayers:
Suppresses hurt sounds of other players on your client.

#### PacketCanceling:
Cancels specific server packets to reduce KB consistency or bypass flags.

#### S00PacketKeepAlive
- **CancelType:** None / OnlyOnGround / OnlyInAir / Always  
- **PacketCount:** 6

#### S32PacketConfirmTransaction
- **CancelType:** None / OnlyOnGround / OnlyInAir / Always  
- **PacketCount:** 1

#### S48PacketResourcePackSend
- **CancelType:** None / OnlyOnGround / OnlyInAir / Always  
- **PacketCount:** Amount of packets to cancel.

---

### Mode: Push

#### PushMode (Simple, Expert):
Determines the method used to reduce knockback.

- **Simple:**  
  Basic, straightforward knockback reduction.

- **Expert:**  
  More advanced, uses hurttime with PushMotion depending on the hurt time.

#### Expert Hurttimes:
There are 10 different modes, each giving different values depending on the hurt time.

#### PushOnGround:
Enables push control only when the player is on the ground.

#### PushMotion:
Controls how much motion is applied when push effects trigger (usually values or parameters affecting movement during knockback).

#### PushStart / PushEnd:
Define when the push effect starts and ends during knockback.

#### OnGround:
Enables push control only when the player is on the ground.

#### NotWhileSPressed:
Disables push control if the sneak (shift) key is pressed.

#### NotWhileLongJump:
Disables push control while performing a long jump to avoid conflicts.

#### Lag:
Adds a delay (in ticks) to the push effect to handle server lag or avoid detection.

#### IgnoreFire:
If enabled, ignores knockback from fire damage sources.

#### CancelDamageSoundsFromOtherPlayers:
Cancels the sound effects from other players' damage to reduce client lag or distraction.

#### Packets To Cancel:
List of packets to cancel (prevent from being sent/processed) to reduce knockback or avoid server detection. Common ones include:

#### 500PacketKeepAlive
- **CancelType:** None / OnlyOnGround / OnlyInAir / Always  
- **PacketCount:** Number of packets to cancel (e.g., 6)

#### S32PacketConfirmTransaction
- **CancelType:** None / OnlyOnGround / OnlyInAir / Always  
- **PacketCount:** Number of packets to cancel (e.g., 1)

#### 548PacketResourcePackSend
**CancelType:** None / OnlyOnGround / OnlyInAir / Always  
- **PacketCount:** Number of packets to cancel