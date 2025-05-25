---
title: ChestStealer
---
Automatically steals items from chests and similar containers. It simulates player clicks to take items quickly and efficiently, often faster than a human player.

### Mode  
Determines the logic used to steal items.  
- Default: Uses standard and consistent logic for safe stealing.  
- Experimental: Uses faster or more randomized behavior to evade detection.

## ModeDeafultTrue

### MinStartDelay  
Minimum delay before starting the steal process.

### MaxStartDelay  
Maximum delay before beginning to steal.

### Instant  
If true, starts stealing instantly without waiting.

### MaxMouseMoveSpeed  
Controls how fast the simulated mouse moves when selecting items.

### MinMouseMoveRandom  
Minimum amount of randomness in the simulated mouse movement.

### MaxMouseMoveRandom  
Maximum amount of mouse movement randomness.

### NotInARow  
Prevents repeating the same pattern for actions to simulate randomness.

### MinCPS  
Minimum clicks per second when interacting with inventory.

### MaxCPS  
Maximum clicks per second allowed.

### MinCPSRecalculate  
Minimum time before recalculating CPS to vary clicking.

### MaxCPSRecalculate  
Maximum time before recalculating CPS.

### MinDoubleClickRate  
Minimum interval to allow occasional double-clicks for realism.

### MaxDoubleClickRate  
Maximum interval for double-clicks.

### MinFailRate  
Minimum chance to simulate failing to grab an item.

### MaxFailRate  
Maximum fail chance.

### MinMissClickRate  
Minimum rate of clicking the wrong slot.

### MaxMissClickRate  
Maximum rate for the same.

### ClickWindow  
Enables using packets to simulate clicks in a more legit-looking way.

### Intelligent  
Loots only useful items first based on prioritization logic.

### ItemBlackList  
List of items that should not be picked up.

### AutoSort  
Automatically sorts items after stealing.

### AutoClose  
Closes chest automatically after the action is complete.

### AutoCloseIfInvFull  
Only closes if the player's inventory is full.

### MinCloseDelay  
Minimum delay before closing the container.

### MaxCloseDelay  
Maximum delay before closing.

### MinChestOpenTime  
Minimum duration to keep chest open for realism.

### MaxChestOpenTime  
Maximum time to keep the chest open.

### WhereToSteal  
Defines container types:  
- Always: All types of containers.  
- ChestsOnly: Only regular Minecraft chests.  
- CustomChest: User-defined or plugin/custom containers.

### ToggleStorageESP  
Highlights containers visually.

### ToggleChestAura  
Automatically loots chests in range.

### Silent  
Steals items without showing the GUI.

### StealIndicator  
Provides visual feedback while stealing.

---
## ModeExperimentalTrue

### MinStartDelay  
How long to wait before starting to steal.

### MaxStartDelay  
Maximum wait time before starting to steal.

### Instant  
If enabled, stealing starts instantly without delay.

### MinCPS  
Minimum clicks per second when stealing items.

### MaxCPS  
Maximum clicks per second when stealing items.

### MinCPSRecalculate  
Minimum delay before recalculating CPS for a more human-like pattern.

### MaxCPSRecalculate  
Maximum delay before recalculating CPS.

### MinDoubleClickRate  
Minimum rate of occasional double-clicks to simulate human input.

### MaxDoubleClickRate  
Maximum rate of double-clicks.

### MinSideStopTicks  
Minimum ticks to pause before stealing from a side slot.

### MaxSideStopTicks  
Maximum ticks to pause for side slot logic.

### MinEmptySlotFailRate  
Minimum chance to fail picking an empty slot, simulating human error.

### MaxEmptySlotFailRate  
Maximum chance for the same.

### RemoveEmptyRows  
Skips empty rows to speed up looting and appear more efficient.

### ClickWindow  
Simulates clicks using packet logic to make the interaction cleaner and legit.

### Intelligent  
Picks valuable or prioritized items first instead of random ones.

### ItemBlackList  
Blocks certain item types from being stolen.

### AutoSort  
Automatically organizes the inventory after stealing.

### AutoClose  
Closes the chest after stealing is done.

### AutoCloseIfInvFull  
Only closes if your inventory is full.

### MinCloseDelay  
Minimum delay before chest is closed after stealing.

### MaxCloseDelay  
Maximum delay before closing.

### MinChestOpenTime  
Minimum time to keep chest open for realism.

### MaxChestOpenTime  
Maximum time to keep chest open.

### WhereToSteal  
Decides which containers can be targeted:  
- Always: Steal from any container.  
- ChestsOnly: Only normal chests.  
- CustomChest: Custom-defined ones.

### ToggleStorageESP  
Turns on ESP for containers to highlight them.

### ToggleChestAura  
Enables automatic interaction and stealing from nearby chests.

### Silent  
Performs stealing without opening the chest GUI.

### StealIndicator  
Shows visual feedback during the stealing process.