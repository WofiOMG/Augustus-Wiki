---
title: MoreKB
---
Manipulates sprint resetting and movement patterns to deal more knockback to opponents. Based on Minecraft knockback mechanics, where sprinting right before hitting causes extra KB. This module controls how, when, and how often sprint is reset for max effect.

### Modes:

### STap
 Classic sprint tapping method: stops and quickly restarts sprint to boost KB.

### LegitSneak
 Simulates sneaking while resetting sprint for stealthy behavior.

### Legit
 Mimics natural sprint resets used by legit players.

### LegitFast
 Same as Legit but with faster timing.

### Fast
 Resets sprint aggressively with minimal delay.

### LessPacket
 Reduces packet usage while resetting sprint to avoid detection.

### Packet
 Uses packet manipulation to reset sprint (no actual key input).

### DoublePacket
 Sends two sprint packets for stronger effect.

### One
 Only does one sprint reset per trigger.



### Duration 

#### MinSprintResetDuration:
Minimum time sprint is canceled before being reset.

#### MaxSprintResetDuration:
Maximum sprint cancel duration.

#### NotInARow:HideSneak Animation:
Hides the sneak animation while using modes like LegitSneak to avoid visual cues.

#### FOV:
Field of view condition – can restrict MoreKB activation to a specific angle/cone of view.

#### IgnoreEatingTargets:
If enabled, ignores targets that are currently eating, to avoid wasted KB boosts.

#### DontSprintResetIfYouAlreadyDidLegit:
Prevents extra sprint resets if a legit-style one was already performed recently. Helps avoid looking suspicious.

#### ## Timing 
MinSprint ResetTime:
Minimum time between sprint reset triggers.

#### MaxSprint ResetTime:
Maximum time between sprint reset triggers. Randomized between min-max to avoid patterns.

### NotInARow:
Prevents sprint resets from happening back-to-back in predictable sequences.

#### MaxInARow:
Sets the maxium number of sprint resets in a row.

### Outliers:
Enables rare “outlier” sprint reset timings outside the normal range to simulate randomness.
MinDoubleResetDelayOutlierValue:
The minimum value used for outlier double reset delay. Only used when an outliner is triggered.

#### MaxDoubleResetDelayOutlierValue:
The maximum value used for outlier double reset delay. Random value is chosen between min and max.

#### MinOutlierDelay:
Minimum delay between two outlier events. Prevents outliers from happening too frequently.

#### MaxOutlierDelay:
Maximum delay between outlier events. Adds randomness to the timing of when outliers can occur.

#### MinSprintResetTimeOutlierValue:
Minimum timing used for rare outlier sprint resets.

#### MaxSprintResetTimeOutlierValue:
Maximum value for outlier reset timings.

#### MinOutlierDelay:
Minimum delay between each outlier reset.

#### MaxOutlierDelay:
Maximum delay between outlier resets.

### Normal Distribution:
Uses a bell-curve distribution (instead of flat randomness) to determine reset timings. Looks more human.
Prevents multiple sprint cancels in a row. Randomizes them to look legit.

#### Sigma:
It controls how spread out or variable the generated values are around the average.

#### Center:
The Center is the mean or average value around which timings cluster.

### Outliers:
Allows unusual durations occasionally for realism.

#### MinSprintResetTicksOutlierValue:
Minimum ticks for sprint to cancel outlier duration.

#### MaxSprintResetTicksOutlierValue:
Maximum ticks for sprint to cancel outlier duration.

#### MinOutlierDelay:
Minimum delay before next outlier event.

#### MaxOutlierDelay:
Maximum delay before next outlier event.

### NormalDistribution:
#### Sigma:
Controls how "spread out" the values are.
Lower values = most reset timings will be close to the center (less variation).
Higher values = more variation and randomness in sprint reset timings.

#### Center:
The average (mean) value for the distribution.
Sprint reset values will tend to cluster around this point when NormalDistribution is enabled.

### DoubleReset 

#### DoubleSprintReset:
Enables back-to-back sprint resets to maximize knockback.

#### MinDoubleResetTiming:
Minimum time between two sprint resets in a double reset.

#### MaxDoubleResetTiming:
Maximum time between sprint resets in a double reset.

#### NotInARow:
Prevents doing multiple double resets consecutively.

#### NomalDistribution:
Randomizes timing between first and second reset with a realistic distribution.

#### Sigma:
Controls the spread of the normal distribution. Higher = more randomness.

#### Center:
Mean value (center) of the distribution for double reset timing.

#### MinDoubleResetDelay:
Minimum delay before another double reset can occur in ticks. 20 ticks= 1 sec

#### MaxDoubleResetDelay:
Maximum delay before another double reset can occur.

### Outliers:
Allows abnormal timing between resets to look more human.

#### MinDoubleResetDelayOutlierValue:
The minimum value used for outlier double reset delay. Only used when an outlier is triggered.

#### MaxDoubleResetDelayOutlierValue:
The maximum value used for outlier double reset delay. Random value is chosen between min and max.

#### MinOutlierDelay:
Minimum delay between two outlier events. Prevents outliers from happening too frequently.

#### MaxOutlierDelay:
Maximum delay between outlier events. Adds randomness to the timing of when outliers can occur.

### Fail

#### FailSprintReset:
Simulates failed sprint resets to avoid perfect patterns. Helps bypass anti-cheat.

#### MinFailDelay:
Minimum delay before a failed sprint reset happens.

#### MaxFailDelay:
Maximum delay before a failed reset.

#### MinFailDuration:
Shortest possible fail duration (how long the sprint reset fails).

#### MaxFailDuration:
Longest possible fail duration.

#### NotInARow:
Avoids multiple failed resets in a row.

### Normal Distribution:
#### Sigma:
Controls how "spread out" the values are.
Lower values = most reset timings will be close to the center (less variation).
Higher values = more variation and randomness in sprint reset timings.

#### Center:
The average (mean) value for the distribution.
Sprint reset values will tend to cluster around this point when NormalDistribution is enabled.
