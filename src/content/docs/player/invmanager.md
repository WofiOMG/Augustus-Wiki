---
title: InvManager
---
Automatically sorts and manages your inventory.

Defines what inventory actions are done automatically.
Options: Sort, Armor, Clean, Craft, HotbarArmor.

### Mode
Controls how inventory is managed.
Options: OpenInv (only when inventory open), SpoofInv (pretends inventory open), SpoofInvOther (spoofs other inventory), Basic (simple management).

#### MinStartDelay
Minimum delay before starting inventory management.

#### MaxStartDelay
Maximum delay before starting inventory management.

#### BlockInputWhileManaging
Prevents player from doing other actions while managing inventory.

#### Visualize
Shows a visual indicator for inventory management.

#### NotWhileScaffold
Disables inventory management while scaffolding.

#### StopMovements
Stops player movement while managing inventory.

#### StopSprinting
Stops sprinting while managing inventory.

### SortInstant
Whether sorting happens instantly.

### InstantFalse

#### MaxMouseMoveSpeed
Maximum speed for mouse movement during sorting.

#### MinMouseMoveRandom
Minimum random variation in mouse movement.

#### MaxMouseMoveRandom
Maximum random variation in mouse movement.

#### MinCPS
Minimum click speed during sorting.

#### MaxCPS
Maximum click speed during sorting.

#### NotInARow
Whether clicks are spaced randomly (not in a row).

#### MinCPSRecalculate
Minimum recalculated click speed.

#### MaxCPSRecalculate
Maximum recalculated click speed.

#### MinFailRate
Minimum chance to fail a click (for human-like behavior).

#### MaxFailRate
Maximum chance to fail a click.

### SortSequence
Order in which items are sorted.
Options: Basic, Nearest, Random.
Basic: sorts items in a simple default order.  
Nearest: chooses items closest to the player’s current slot.  
Random: picks items in a random order to seem less predictable.

### Slots
Defines what type of items go in each hotbar slot.
Options per slot: None, Sword, Bow, Rod, Throwables, Blocks, EnderPearls, Food, Gapple, Soups.

### ArmorNoArmorDrop
Whether to drop armor automatically.

### OnlyInHotbar
Restricts armor management to hotbar slots only.

### IgnoreDurability
Ignores item durability when managing armor.

### ArmorInstant
Whether armor switching is instant.

#### Armor MaxMouseMoveSpeed
Max mouse speed while managing armor.

#### ArmorMinMouseMoveRandom
Min mouse movement randomness for armor.

#### ArmorMaxMouseMoveRandom
Max mouse movement randomness for armor.

#### ArmorMinCPS
Min clicks per second when managing armor.

#### ArmorMaxCPS
Max clicks per second when managing armor.

#### ArmorNotInARow
Whether armor clicks are spaced randomly.

#### ArmorMinCPSRecalculate
Minimum recalculated CPS for armor.

#### ArmorMaxCPSRecalculate
Maximum recalculated CPS for armor.

#### ArmorMinDoubleClickRate
Minimum double-click rate for armor.

### ArmorMaxDoubleClickRate
Maximum double-click rate for armor.

#### ArmorMinFailRate
Minimum chance to fail armor clicks.

#### ArmorMaxFailRate
Maximum chance to fail armor clicks.

#### ArmorMinMissClickRate
Minimum chance to miss a click while managing armor.

#### ArmorMaxMissClickRate
Maximum chance to miss a click while managing armor.

### ArmorSequence
Order in which armor pieces are equipped or unequipped.
Options: Basic, Nearest, Random.

### Cleane KeepAllArmor
Whether to keep all armor during cleaning.

### CleanerInstant
Whether cleaning happens instantly.

#### CleanerMaxMouseMoveSpeed
Max mouse speed during cleaning.

#### CleanerMinMouseMoveRandom
Min mouse movement randomness for cleaning.

#### CleanerMaxMouseMoveRandom
Max mouse movement randomness for cleaning.

#### CleanerMinCPS
Min clicks per second during cleaning.

#### CleanerMaxCPS
Max clicks per second during cleaning.

#### CleanerNotInARow
Whether cleaning clicks are spaced randomly.

#### CleanerMinCPSRecalculate
Min recalculated CPS during cleaning.

#### CleanerMaxCPSRecalculate
Max recalculated CPS during cleaning.

#### CleanerMinFailRate
Min chance to fail a click during cleaning.

#### CleanerMaxFailRate
Max chance to fail a click during cleaning.

#### CleanerMinMissClickRate
Min chance to miss a click during cleaning.

#### CleanerMaxMissClickRate
Max chance to miss a click during cleaning.

### CleanerSequence
Order in which items are cleaned.
Options: Basic, Nearest, Random.

### ItemStackLimits
Limits for how many of certain items can be stacked in inventory.

- BlockStackLimit: Max blocks per stack.
- FoodStackLimit: Max food per stack.
- WaterBucketLimit: Max water buckets per stack.
- LavaBucketLimit: Max lava buckets per stack.
- ThrowablesLimit: Max throwable items per stack.

### ClickMode
Mode used for clicking during inventory management.