---
title: FastBreak
---

### NoBlockHitDelay:  
Removes the vanilla cooldown between block hits. Allows instant repeated breaking. Vanila is 5 ticks.

### IgnoreMiningFatigue:  
Ignores Mining Fatigue effects. You break blocks at full speed even with the debuff.

### OnlyWhenBlink:  
Only applies the effect when the Blink module is active. Useful for stealth mining.

### IgnoreBeds:  
Prevents the module from affecting beds. Helps beds not respawning after getting broken.

### DebugBreakSpeed:  
Shows debug info about your mining speed. Use for testing or fine-tuning settings.

### Mode: Simple, Expert  
- **Simple**: One multiplier for all tools/blocks.  
- **Expert**: Lets you set different speeds per item or block type. More precise, flags less.

#### CustomInAirMultiplier:  
Allows modifying break speed while you're in the air (normally slower in vanilla).

#### InAirMultiplier:  
The multiplier used when you're mining in the air.

#### Multiplier:  
The global block breaking speed multiplier. Affects how fast blocks break overall.

#### ArtificialMiningSpeedEffect:  
Simulates effects like Haste. Acts as if you have a mining speed potion, even if you don’t.

#### Instant:  
If true, blocks that meet the speed threshold will break instantly — like in creative mode.

### DedicatedItemHandling:
Only use FastBreak when you have the specefied tool in your current hotbar slot.