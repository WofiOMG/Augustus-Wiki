# PING
Simulates controlled ping behavior by delaying both incoming and outgoing packets, often used for synchronization exploits, bypasses, or custom behavior in combat.

## IncomingGroup
Controls simulated delay for packets from server to client.

**MinIncomingPing**
Minimum delay (in milliseconds) applied to incoming packets.

**MaxIncomingPing**
Maximum delay (in milliseconds) applied to incoming packets.

**MinPingRecalculateDelay**
Minimum delay between recalculating a new simulated ping value.

**MaxPingRecalculateDelay**
Maximum delay between ping recalculations.

**PingAccelerationMode**
Defines how ping changes over time — Instant applies changes immediately, Smooth gradually applies them.

**MinPingAccelerationPerSecond**
Minimum rate of increase for ping per second.

**MaxPingAccelerationPerSecond**
Maximum rate of increase for ping per second.

**MinPingAccelerationApplyDelay**
Minimum time before the next ping acceleration can apply.

**MaxPingAccelerationApplyDelay**
Maximum delay before applying the ping acceleration.

**MinPingAccelerationRecalculateDelay**
Minimum interval between recalculations of acceleration behavior.

**MaxPingAccelerationRecalculateDelay**
Maximum interval between acceleration recalculations.

**MinPingDecelerationTime**
Minimum time needed to reduce the simulated ping smoothly.

**MaxPingDecelerationTime**
Maximum allowed time to decelerate the ping to a lower value.

## OutgoingGroup
Controls simulated delay for packets from client to server.

**MinOutgoingPing**
Minimum simulated ping on outgoing packets.

**MaxOutgoingPing**
Maximum simulated ping on outgoing packets.

**MinPingRecalculateDelay**
Minimum delay before recalculating the outgoing ping.

**MaxPingRecalculateDelay**
Maximum delay between outgoing ping recalculations.

**PingAccelerationMode**
Controls how outgoing ping transitions — Instant or Smooth.

**MinPingAccelerationPerSecond**
Minimum speed at which ping increases per second.

**MaxPingAccelerationPerSecond**
Maximum speed at which ping increases per second.

**MinPingAccelerationApplyDelay**
Shortest wait before acceleration is applied to outgoing packets.

**MaxPingAccelerationApplyDelay**
Longest wait before acceleration is applied.

**MinPingAccelerationRecalculateDelay**
Shortest delay before recalculating acceleration behavior.

**MaxPingAccelerationRecalculateDelay**
Longest delay before recalculating acceleration.

**MinPingDecelerationTime**
Minimum duration for reducing ping smoothly.

**MaxPingDecelerationTime**
Maximum duration for gradual ping reduction.

**CombatMode**
Enables special behavior or packet delays when engaged in combat.

**MinPingStartDelay**
Delay before starting ping simulation when combat begins.

**MaxPingStartDelay**
Maximum delay before activating ping logic during combat.

**ResetPingAtDistanceToTarget**
Resets simulated ping behavior if the player is too far from the target.

**FailRate**
Introduces randomization or failure chances in simulation.

**MinFailInterval / MaxFailInterval**
Controls the interval between potential simulated failures.

**Targets**
Specifies which entities are affected by or taken into account during ping manipulation:

Player, Mob, Animal, Villager, ArmorStand

**FlushConditions**
Triggers an immediate flush of all delayed packets under specific actions to avoid desync or misbehavior:

StandingStill
ScaffoldToggled
PlaceBlocks
BreakBlocks
HoldingBlocks
UseItem
OpenedGUI
InventoryActions
Velocity
Explosion
Teleport
SprintReset
SplashPotion
Attack