---
title: BackTrack
---
Lets you hit players where they were a few ticks ago, bypassing latency or desync by attacking their past positions.

### Mode
Selects how backtracking is applied:

---
### BackTrack
Standard mode.

----
### LagTrack
Focused on compensating server lag.

---
### Gomme
Tuned for GommeHD.

---
### Ping
Adjusts based on ping delay.

---
### ClassicBackTrack
Legacy behavior.

### AllModes:

#### MaxBackTrackRangeMin / MaxBackTrackRangeMax
Sets the range in blocks where backtracking will consider positions.

#### Threshold
Minimum distance the target must have moved to trigger a backtrack.

#### CancelHitsIfServerCancelsHit
Prevents repeated hitting if server cancels a hit.

#### MinBackTrackDelay / MaxBackTrackDelay
Delay before a backtrack attempt is made.

#### MinDelayBetweenBacktracks / MaxDelayBetweenBacktracks
Sets a delay between two backtracking attempts.

#### Subtract ping from Delay
Reduces the delay time based on your current ping. Use this to have the same ping in PvP if your original ping is 50 or 100.

#### ForceDelay
Forces use of delay even when not needed.

#### Predict
Predicts target movement to improve accuracy.

#### Dynamic
Dynamically adjusts the backtrack based on current server and ping conditions.

#### CheckStartDistance
Enables a check for distance before backtracking.

#### AbortCriterion
Defines when to cancel backtrack:

#### None
BackTrack wont be canceled.

#### OnAttack
BackTrack will be canceled on first hit on your opponent.

#### OnRange
BackTrack will be canceled when in a certain range from opponent. Useful to stop backtrack while very close to the enemy.

#### FixPacketOrder
Reorders packets to avoid timing issues.

#### StopOnAttackMaxHurtTime / StopBackTrackAtHurtTime
Prevents backtracking when targets are recently hit or damaged.

#### NotWhileScaffold
Disables the module while scaffold is active.

#### Improve
Improves target movement prediction accuracy.

#### OnlyKillAura
Only activates when KillAura is enabled. Don’t use this if you don’t use KillAura or backtrack won’t work.

#### Targets
Selects which entities can be backtracked:
Player, Mob, Animal, Villager, ArmorStand
Not using AntiBot might result the backtrack to work on bots such as shopkeepers.

#### PreAimRange
Sets the range within which to start aiming at a backtracked target.

### ClickCheck
Only works if clicks are registered (used for legit behavior).

### Mode: LagTrack

#### ClickCheck
Only works if clicks are registered (used for legit behavior).

#### Mode: LagTrack

#### MaxBackTrackRangeMin / MaxBackTrackRangeMax
Defines the minimum and maximum range (in blocks) to track targets' past positions.

#### Threshold
Minimum movement distance for a target to be considered lagging.

#### CancelHitsIfServerCancelsHit
Prevents hits if the server has canceled a previous one.

#### MinMaxLagPackets / MaxMaxLagPackets
Sets the minimum and maximum number of lag packets to wait for before executing a backtrack.

#### NotInARow
Avoids executing lagtrack back-to-back.

#### DelayBetweenLags
Sets delay (ms) between two lag-based backtrack attempts.

#### CountMode
Defines how to count lag packets:

#### Tick
Based on game ticks.

#### MovePacket
Based on movement packet frequency.

#### Subtract ping from Delay
Subtracts your ping from the configured delay for better accuracy.

#### CheckStartDistance
Ensures the target is far enough to make lag-back logical.

#### AbortCriterion
Defines when to stop the lagtrack attempt.

#### None
BackTrack won’t be canceled.

#### OnAttack
BackTrack will be canceled on first hit on your opponent.

#### OnRange
BackTrack will be canceled when in a certain range from opponent. Useful to stop backtrack while very close to the enemy.

#### FixPacketOrder
Ensures correct packet order when simulating lag.

#### StopOnAttackMaxHurtTime
Stops the module if the target's HurtTime exceeds a set threshold (e.g., 6).

#### StopBackTrackAtHurtTime
Disables if the target was recently hit.

#### NotWhileScaffold
Disables when scaffold is active.

#### Improve
Enables improved prediction and calculation logic.

#### OnlyKillAura
Only activates when KillAura is enabled. LagTrack won’t work at all if you don’t use KillAura.

#### Targets
Entities that can be lagtracked:
Player, Mob, Animal, Villager, ArmorStand
Not using AntiBot can cause lagtrack to activate on bots such as shopkeepers if conditions meet.

#### PreAimRange
Distance at which aim begins for the lagtracked position.

#### ClickCheck
Activates only if the player is actively clicking (for legit-like behavior).

---
### Mode: Gomme

#### MaxBackTrackRangeMin / MaxBackTrackRangeMax
Defines the minimum and maximum distance (in blocks) to look back at a target’s past position.

#### Threshold
Minimum positional difference for a backtrack to trigger.

#### CancelHitsIfServerCancelsHit
Prevents hitting if the server rejects a previous hit.

#### MaxLagPackets
Maximum lag packets allowed before attempting a backtrack.

#### CheckStartDistance
Normally checks if the target was far enough before lagging.

#### AbortCriterion
Defines when to cancel backtrack attempts:

#### None
BackTrack won’t be canceled.

#### OnAttack
BackTrack will be canceled on first hit on your opponent.

#### OnRange
BackTrack will be canceled when in a certain range from opponent. Useful to stop backtrack while very close to the enemy.

#### FixPacketOrder
Fixes the sequence of packets to prevent detection.

#### StopOnAttackMaxHurtTime
Stops if the target's hurt time exceeds the value (e.g., 6 ticks).

#### StopBackTrackAtHurtTime
Disables backtracking if the target is still in the hurt state.

#### NotWhileScaffold
Prevents BackTrack from activating while Scaffold is running.

#### Improve
Enables smarter calculations and hit prediction.

#### OnlyKillAura
BackTrack only works if KillAura is enabled. Gomme mode backtrack will not work at all if KillAura isn’t enabled.

#### Targets
Specifies which entities are valid targets:  
Player, Mob, Animal, Villager, ArmorStand  
Not using AntiBot can cause Gomme mode backtrack to attack bots such as shopkeepers when conditions are met.

#### PreAimRange
Range at which aim adjusts to lagged positions.

#### ClickCheck
Only runs when player is clicking (helps with legit bypass).

---
### Mode: Ping

#### MaxBackTrackRangeMin / MaxBackTrackRangeMax
Sets the range of how far back (in blocks) positions are considered.

#### Threshold
Minimum movement change to trigger backtrack.

#### CancelHitsIfServerCancelsHit
Cancels attacks if the server previously rejected a hit.

#### MinPingDelay / MaxPingDelay
Delays backtrack actions based on your ping. The module chooses a delay between these two values.

#### Delay BetweenBacktracks
Minimum time (in ms) between two backtrack actions.

#### Subtract own ping from Delay
Compensates for your own latency in delay calculations. Very useful especially for public configs or non-stable connections.

#### Dynamic
Enables adaptive delay based on network conditions.

#### CheckStartDistance
Checks if target was far enough before backtracking.

#### AbortCriterion
Cancels backtrack if:

#### None
BackTrack won’t be canceled.

#### OnAttack
BackTrack will be canceled on first hit on your opponent.

#### OnRange
BackTrack will be canceled when in a certain range from opponent. Useful to stop backtrack while very close to the enemy.

#### FixPacketOrder
Prevents detection by reordering outgoing packets correctly.

#### StopOnAttackMaxHurtTime
Stops backtracking if target is still in hurt state longer than this value (e.g., 6 ticks).

#### StopBackTrackAtHurtTime
Prevents backtracking when the entity is still hurt.

#### NotWhileScaffold
Disables backtracking while Scaffold module is active.

#### Improve
Enables prediction and better positioning logic.

#### OnlyKillAura
BackTrack activates only when KillAura is active.

#### Targets
Applies backtracking to:  
Player, Mob, Animal, Villager, ArmorStand

#### PreAimRange
How close the aim must be to a backtracked position to apply it.

#### ClickCheck
Only allows backtrack when player is clicking (for legit look).

### Mode: ClassicBackTrack

#### MaxBackTrackRangeMin / MaxBackTrackRangeMax
Sets how far back (in blocks) a target’s position can be reverted to.

#### Threshold
Minimum position change required to trigger a backtrack.

#### CancelHitsIfServerCancelsHit
Cancels the hit attempt if the server rejects the last one.

#### MinBackTrackDelay / MaxBackTrackDelay
Sets a fixed delay range (in ms) for how long the module should wait before applying a backtrack.

#### OnlyWhenNeed
Activates only when needed (e.g., when the target moves unpredictably or hit fails). Reduces unnecessary usage.

#### Dynamic
Enables adaptive delay handling depending on combat conditions.

#### NotWhileScaffold
Disables ClassicBackTrack while Scaffold is active.

#### Improve
Applies better prediction and positioning logic.

#### OnlyKillAura
BackTrack only works while KillAura is enabled.

#### Targets
Backtrack will apply to:  
Player, Mob, Animal, Villager, ArmorStand  
ClassicBackTrack might be activated on bots such as shopkeepers if not using AntiBot.

#### PreAimRange
Distance within which your crosshair must be near the backtracked position for the hit to register.

#### ClickCheck
Ensures backtrack only happens while the player is actively clicking (for more legit behavior).