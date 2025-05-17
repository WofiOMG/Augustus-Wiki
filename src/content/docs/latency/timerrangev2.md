# TIMERRANGERV2
TimerRangeV2 is an enhanced timer manipulation module. It controls how your game ticks (server updates) are sped up or slowed down dynamically, especially during combat, to improve hit registration and synchronization while trying to remain undetected by anti-cheats.

**DynamicLagTicks:**
Enables dynamic adjustment of lag ticks to better sync timer changes with lag.

**LagTickDiff:**
The difference in lag ticks allowed before adjusting timer behavior.

**TimerTicks:**
Number of timer ticks to speed up or slow down per cycle.

**MaxTargetHurttime:**
Maximum hurt time of a target entity to consider for timer manipulation.

**Delay:**
Sets delay before timer manipulation activates or repeats.

**Correct:**
Enables correction for timer adjustments to avoid desync.

**Dynamic:**
When enabled, timer adapts dynamically based on conditions (false means fixed).

**Accurate:**
Ensures the timing adjustments are precise.

**Debug:**
Enables debug mode to display timing info for troubleshooting or just chat cosmetic.

**OnlyOnGround:**
Timer manipulations only activate when player is on the ground.

**FixMode:**
Select fix mode for timer behavior: None, Fix1, or Fix2 (explained before).

**Extreme:**
An option for aggressive timer manipulation (details depend on implementation).

**Targets:**
Defines which entities the module should consider for timer effects.

**OnlyWhileKillAura:**
Module activates only when KillAura (auto attack) is active.

**PreAimRange:**
Range in blocks to pre-aim for targets before applying timer manipulation.