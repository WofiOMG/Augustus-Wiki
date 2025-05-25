---
title: LagRange
---
Simulates lag spikes by delaying and correcting position to manipulate hit registration or confuse server-side detection.

### PredictTicks
How many ticks ahead the module predicts movement.

### Ticks
Duration of the simulated lag spike in ticks.

### Correct
If true, repositions you correctly after the lag.

### OnlyOnGround
Only activates while you're on the ground.

### Stop
Stops the lag behavior after conditions are met.

#### STap
Applies short tap-lag correction logic.

### Delay after attack
How long to wait (in ms) after an attack before activating LagRange.

### Delay between lags
Minimum time (in ms) between two LagRange activations.

### Stop early
Stops LagRange early after this many ticks if conditions are met.

### Targets

### OnlyWhileKillAura
Works only when KillAura is enabled.

#### Targets
List of valid targets (Player, Mob, Animal, Villager, ArmorStand).

#### PreAimRange
Distance at which pre-aiming starts.

### Debug
Enables debug output.

### OnlyInThirdPerson
Shows debug only in 3rd-person view.

### Time debug gets displayed
Duration (in seconds) to show debug info on screen.