---
title: Criticals
---
Improves the chance to land critical hits by manipulating movement and sprinting conditions during attacks.

### Modes: IntaveLowHop
Performs a very small jump (low hop) to trigger critical hits, designed to bypass Intave anti-cheat.

---
### Packet
Sends specific packets to the server to fake the upward movement needed for critical hits without actually jumping.

---
### Lag
Simulates lag to create the timing window for critical hits, useful on servers sensitive to movement.

---
### NoGround
Tricks the server into thinking you are airborne without jumping, allowing critical hits without leaving the ground visually.

---
### CustomPacket
Allows custom configuration of packets to tailor critical hit triggering based on server specifics.

---
### PacketEdit
Modifies outgoing packets related to movement to induce critical hit conditions.

---
### Modes: IntaveLowHop, Packet

#### LagDuration
Sets how long the module simulates lag to time critical hits better, improving success rate during network delays.

#### ForceHit
Forces critical hit conditions even when they normally wouldn’t occur, increasing the chance to trigger critical hits artificially.

#### MoveSlowdownOnGround
Controls whether your movement slows down on the ground during critical attacks.

#### SprintOnGround
Enables sprinting while on the ground during critical hits.

#### MoveSlowdownInAir
Controls movement slowdown while in the air during critical hits.

#### SprintOnGroundInAir
Allows sprinting both on the ground and in the air during critical hits.

#### Smart
Automatically adjusts critical hit conditions based on the situation to optimize performance.

---
### Mode: Lag

#### LagDuration
Sets how long the module simulates lag to time critical hits better, improving success rate during network delays.

#### ForceHit
Forces critical hit conditions even when they normally wouldn’t occur, increasing the chance to trigger critical hits artificially.

#### Mode: NoGround

#### OnlyOnHit
Whether to activate NoGround mode only when hitting a target.

#### Floating
Makes the player appear slightly floating to the server, aiding in critical hit triggering.

#### LagDuration
Duration (in ticks) to simulate lag when using NoGround mode to improve critical hit timing.

#### ForceHit
Forces the critical hit effect even when normal conditions aren’t met.

#### OnlyWhileJumpKeyPressed
Activates NoGround mode only if the jump key is held down.

#### OnlyWhileKillAuraTarget
Enables NoGround mode only when attacking a KillAura target. Keep this off if you are using other aim hacks.

#### CriticalsInAir
(Usually true) Allows critical hits to occur while airborne.

#### CriticalsOnGround
Allows critical hits to be registered even when on the ground.

---
### CustomPacket

#### UseC06
Whether to use a specific packet type (C06) for movement updates.

#### Interval
How often the custom packets are sent (in ticks).

#### SendFirst
Whether to send the first movement packet in the sequence.

#### OnGroundFirst
Whether the first packet reports the player as on the ground.

#### MinYAddFirst
Minimum vertical offset added to the first packet to simulate slight upward movement.

#### MaxYAddFirst
Maximum vertical offset added to the first packet.

#### SendSecond
Whether to send the second movement packet.

#### OnGroundSecond
Whether the second packet reports the player as on the ground.

#### MinYAddSecond
Minimum vertical offset added to the second packet.

#### MaxYAddSecond
Maximum vertical offset added to the second packet.

#### SendThird
Whether to send the third movement packet.

#### OnGroundThird
Whether the third packet reports the player as on the ground.

#### MinYAddThird
Minimum vertical offset added to the third packet.

#### MaxYAddThird
Maximum vertical offset added to the third packet.

#### SendFourth
Whether to send the fourth movement packet.

#### OnGroundFourth
Whether the fourth packet reports the player as on the ground.

#### MinYAddFourth
Minimum vertical offset added to the fourth packet.

#### MaxYAddFourth
Maximum vertical offset added to the fourth packet.

#### LagDuration
Duration of simulated lag to optimize critical hit timing.

#### ForceHit
Forces critical hit conditions even if natural triggers aren’t met.

#### OnlyWhileJumpKeyPressed
Activates packet sending only when the jump key is held.

#### OnlyWhileKillAuraTarget
Enables the mode only when attacking a KillAura target.

#### CriticalsInAir
Allows critical hits while airborne.

#### CriticalsOnGround
Allows critical hits while on the ground.

---
### PacketEdit

#### OnlyOnHit
Activates the mode only when hitting a target.

#### SetOnGroundToFalse
Changes the "on ground" status in packets to false, making the server think the player is airborne.

#### MinYadd
Minimum vertical offset added to packets to simulate upward movement.

#### MaxYadd
Maximum vertical offset added to packets.

#### LagDuration
Simulates lag duration to improve timing for critical hits.

#### ForceHit
Forces critical hit conditions even if normal triggers aren’t met.

#### OnlyWhileJumpKeyPressed
Enables mode only if the jump key is pressed.

#### OnlyWhileKillAuraTarget
Enables mode only when attacking a KillAura target.

#### CriticalsInAir
Allows critical hits while airborne.

#### CriticalsOnGround
Allows critical hits while on the ground.