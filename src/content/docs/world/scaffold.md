---
title: Scaffold
--- 
One of the most important modules for many players, Scaffold lets you automatically place blocks beneath you while moving, making building bridges or towers fast and safe. Just like KillAura is vital for combat, Scaffold is a for anyone who wants to build quickly without worrying about falling.

You can see your player’s rotations in third-person view (both front and back) which helps you understand how the module targets block placement. In first-person view, rotations aren’t visible because you’re seeing through the player’s eyes, but the module still perfectly handles aiming and block placement behind the scenes. Rotations happen only server side in first-person view.

# RotationSpeeds

### ModeNew  
Determines whether to use the new rotation mode or the old/default one. False means old mode is used.

## ModeNewTrue
Easy to use but very inefficient.

### AimSpeed
Controls overall (Y, X, Z) aim speed.

## ModeNewFalse

### MinYawSpeed  
Minimum horizontal (yaw) rotation speed.

### MaxYawSpeed  
Maximum horizontal (yaw) rotation speed.

### MinPitchSpeed  
Minimum vertical (pitch) rotation speed.

### MaxPitchSpeed  
Maximum vertical (pitch) rotation speed.

### MinYawAcceleration  
Minimum acceleration for yaw rotation.

### MaxYawAcceleration  
Maximum acceleration for yaw rotation.

### MinPitchAcceleration  
Minimum acceleration for pitch rotation.

### MaxPitchAcceleration  
Maximum acceleration for pitch rotation.

### CustomBlockClutchRotationSpeeds  
Enables use of custom rotation speeds for block clutch action when true.

## CustomBlockClutchRotationSpeedsTrue
Give better control over rotation speed when clutching blocks. (false uses same clutch rotation as normal rotation)

## BlockClutchModeNew  
Rotation mode used during block clutch; false means old mode.

### BlockClutchModeNewTrue
Easy to use but very inefficient.

#### AimSpeed
Control overall (Y, X, Z) aim speed.

## BlockClutchModeNewTrue
Use a way better clutch mode.

### BlockClutchMinYawSpeed  
Minimum yaw speed during block clutch.

### BlockClutchMaxYawSpeed  
Maximum yaw speed during block clutch.

### BlockClutchMinPitchSpeed  
Minimum pitch speed during block clutch.

### BlockClutchMaxPitchSpeed  
Maximum pitch speed during block clutch.

### BlockClutchMinYawAcceleration  
Minimum yaw acceleration during block clutch.

### BlockClutchMaxYawAcceleration  
Maximum yaw acceleration during block clutch.

### BlockClutchMinPitchAcceleration  
Minimum pitch acceleration during block clutch.

### BlockClutchMaxPitchAcceleration  
Maximum pitch acceleration during block clutch.

## MinKeepRotationsAfterModuleDisable  
Minimum rotation preserved after disabling the rotation module.

## MaxKeepRotationsAfterModuleDisable  
Maximum rotation preserved after disabling the rotation module.

# RotationRandomizationV
Enables or controls randomization of rotations for both pitch and yaw.

### RandomizePitch  
Enables randomization of pitch (vertical) rotation when true.

### RandomizePitchChanceWhileYawRotation  
Chance (percentage) to randomize pitch while yaw rotation is occurring.

### RandomizePitchChanceOnBlock  
Chance (percentage) to randomize pitch while blocking.

### RandomizePitchChanceInAir  
Chance (percentage) to randomize pitch while in the air.

### OtherPitchRandomization  
Settings related to additional pitch randomization parameters.

## OtherPitchRandomizationFalse

### MinRandomizePitchVal  
Minimum value for random pitch adjustment.

### MaxRandomizePitchVal  
Maximum value for random pitch adjustment.

### MinRandomizePitchInterval  
Minimum interval between pitch randomizations.

### MaxRandomizePitchInterval  
Maximum interval between pitch randomizations.

### NotInARow  
Prevents pitch randomization from happening consecutively.

## RandomizeYaw  
Enables randomization of yaw (horizontal) rotation when true.

## RandomizeYawTrue

### RandomizeYawChanceWhilePitchRotation  
Chance (percentage) to randomize yaw while pitch rotation is occurring.

### RandomizeYawChanceOnBlock  
Chance (percentage) to randomize yaw while blocking.

### RandomizeYawChanceOnAir  
Chance (percentage) to randomize yaw while in the air.

### OtherYawRandomization  
Settings related to additional yaw randomization parameters.

## OtherYawRandomizationFalse

### MinRandomizeYawVal  
Minimum value for random yaw adjustment.

### MaxRandomizeYawVal  
Maximum value for random yaw adjustment.

### MinRandomizeYawInterval  
Minimum interval between yaw randomizations.

### MaxRandomizeYawInterval  
Maximum interval between yaw randomizations.

### NotInARow  
Prevents yaw randomization from happening consecutively.

# StaticPitchSettings  
Contains settings for applying static pitch angles during movement, jumps, and clutches.
Locks your vertical view angle (pitch) at a set value, usually around 80°, to keep your aim steady. It’s used for clutching, bridging, and bypassing anti-cheat by making movement look consistent and legit.

### StaticPitch  
Enables the use of a static pitch angle.

### StaticPitchAtJump  
Applies static pitch while jumping.

### StaticPitchRandomizeOnlyAtStart  
Randomizes static pitch only at the start of the action, not continuously.

### IgnoreStaticPitchForBlockClutches  
If true, disables static pitch during block clutch actions.

### MinStaticPitchForward  
Minimum pitch angle when facing forward using static pitch.

### MaxStaticPitchForward  
Maximum pitch angle when facing forward using static pitch.

### StaticPitchDiagonal  
Enables static pitch while moving diagonally.

### StaticPitchAtJumpDiagonal  
Applies static pitch during diagonal jumps.

### StaticPitchRandomizeOnlyAtStartDiagonal  
Only randomizes static pitch at the beginning of diagonal movement.

### IgnoreStaticPitchForBlockClutchesDiagonal  
Disables static pitch for diagonal block clutch actions if true.

### MinStaticPitchDiagonal  
Minimum pitch angle for diagonal movement.

### MaxStaticPitchDiagonal  
Maximum pitch angle for diagonal movement.

## RotationForStaticPitch
### ReduceYawRotation  
Reduces how much yaw (horizontal angle) is rotated during movement.

### StrictYaw  
Enables strict yaw constraints for more accurate or limited movement.

#### MinStrictYawIncorrectFactor  
Minimum factor allowed for incorrect yaw deviation.

#### MaxStrictYawIncorrectFactor  
Maximum factor allowed for incorrect yaw deviation.

#### MinStartDelayAfterDirectionChange  
Minimum delay before applying rotation after changing movement direction.

#### MaxStartDelayAfterDirectionChange  
Maximum delay before applying rotation after changing movement direction.

### RotateWithMovement  
Enables rotation based on player movement.

### RotateWithMovementOnlyOrthogonal  
Only rotates with movement when the direction is orthogonal (not diagonal).

### Improve  
Enables general improvements to rotation and prediction logic.

#### ImproveOnlyAtClutch  
Applies improvement logic only during clutch situations.

### ExtraBlockSearch  
Expands the block search range to find more clutch placements.

#### ExtraBlockSearchOnlyAtClutch  
Only uses extended block search during clutching.

## Strafe
Enables strafing movement while bridgeing (not diagonally).

## StrafeTrue

### MinStrafeDegree
Defines the minimum angle (in degrees) for strafing.

### MaxStrafeDegree
Defines the maximum angle (in degrees) for strafing.

### MinStrafeWidth
Controls the minimum side-to-side distance of each strafe movement.

### MaxStrafeWidth
Controls the maximum side-to-side distance of each strafe movement.

### CorrectRotationWhileBuilding
Keeps your rotation accurate and aligned during building.

## CorrectStrafeWithKeyBinds
Adjusts strafe direction based on pressed movement keys.

### CorrectStrafeWithKeyBindsCage
Strafes correctly when in cage situations (e.g., box starts or void clutches).

### MinCorrectStrafeWithKeyBindsWidth
Sets the minimum width of the correction strafe when using keybinds.

### MaxCorrectStrafeWithKeyBindsWidth
Sets the maximum width of the correction strafe when using keybinds.

### MinCorrectStrafeWithKeyBindsDuration
Defines the minimum duration (in ticks) of keybind correction.

### MaxCorrectStrafeWithKeyBindsDuration
Defines the maximum duration (in ticks) of keybind correction.

### NotInARow
Prevents the same correction pattern from happening repeatedly.

### MinCorrectStrafeWithKeyBindsMiddle
Minimum offset from center used during keybind-based strafing.

### MaxCorrectStrafeWithKeyBindsMiddle
Maximum offset from center used during keybind-based strafing.

### MinCorrectStrafeWithKeyBindsMiddleExclusion
Minimum excluded zone where middle strafe should not activate.

### MaxCorrectStrafeWithKeyBindsMiddleExclusion
Maximum excluded zone where middle strafe should not activate.

### MinDelayToRecalculateMiddle
Minimum delay before recalculating the middle strafe position.

### MaxDelayToRecalculateMiddle
Maximum delay before recalculating the middle strafe position.

### StartAtEdge
Starts rotation behavior when the player is at the edge of a block.

#### MinStartAtEdgeDelay
Minimum delay before triggering rotation at edge.

#### MaxStartAtEdgeDelay
Maximum delay before triggering rotation at edge.

### IgnoreStartAtEdgeAtBlockClutch
Ignores edge start behavior during block clutching.

### EdgeRotateCheck
Checks if rotation should be adjusted when near an edge.

#### EdgePlaceCheck
Checks if block placement is aligned with the edge.

### Flick
Enables fast flick-like rotation for quick reaction or block placement.

#### OtherFlick
Enables secondary flick behavior (e.g., for fallback or secondary logic).

### OtherRotation
Enables additional rotation logic for smoother transitions.

### RecycleRotation
Reuses previous rotation angles for more consistent movement.

### Intave
Applies rotation adjustments for compatibility with Intave anti-cheat.

#### IntaveSafe
Uses safer values for Intave to avoid detection.

#### IntaveFast
Uses faster values for Intave if safety allows it.

### PitchSelection
Controls how pitch angle is selected:
Nearest, Furthest, Highest, Lowest, Mid, Random

### MaxPitchCorrection
Maximum amount of pitch correction allowed.

### IgnoreMaxPitchCorrectionIfBlockClutch
Ignores the pitch correction limit when block clutching.

### Expand
Allows expanded or flexible rotation movement when needed.

#### ExpandLenght
Increases how far the system looks for blocks to place or rotate to.

## RotationsForStrafeSettings

### NoSwing
Disables the arm swing animation when clicking.

#### ServerSideNoSwing
Disables the swing animation sent to the server.

### MinCPS
Minimum clicks per second allowed.

### MaxCPS
Maximum clicks per second allowed.

### DCPSMode
InternalDCPSModeTrue: The program decides how fast to click by itself.
ExternalDCPSModeTrue: Something else (like another tool or you) controls how fast it clicks.

### DCPSModeExternalTrue
DCPS= Dynamic clicks per second. 

#### MinDCPS
Minimum dynamic clicks per second. A dynamic click changes its speed automatically based on the situation.

#### MaxDCPS
Maximum dynamic clicks per second. A dynamic click changes its speed automatically based on the situation.

### ForcePlaceIfYouWouldFallDown
Forces block placement if it prevents falling.

### AlwaysPlaceWhenPossible
Always attempts to place blocks when conditions allow.

### ClickPause
Pauses clicking under certain conditions.

### DelayClick
Delays clicks to mimic more natural timing.

### OneClick
Limits to one click per action or tick.

### MaxYawRotationDeltaToPlaceBlocks
Maximum yaw rotation change allowed for block placement.

### MaxPitchRotationDeltaToPlaceBlocks
Maximum pitch rotation change allowed for block placement.

### RemoveRotationDeltaLimitAtBlockClutch
Removes rotation limits during block clutch moves.

## Sneaking
Enables sneaking.

### TimeJumpForOneStackForward
Allows a time jump when sneaking one block forward.

### OneStackForward
Sneaks exactly one block forward.

#### MinMinOffGroundSneakTickForward
Minimum ticks off the ground before sneaking forward (min range).

#### MaxMinOffGroundSneakTickForward
Maximum ticks off the ground before sneaking forward (min range).

### MinMaxOffGroundSneakTickForward
Minimum ticks off the ground before sneaking forward (max range).

#### MaxMaxOffGroundSneakTickForward
Maximum ticks off the ground before sneaking forward (max range).

### OneStackDiagonal
Sneaks exactly one block diagonally.

#### MinMinOffGroundSneakTickDiagonal
Minimum ticks off the ground before sneaking diagonally (min range).

#### MaxMinOffGroundSneakTickDiagonal
Maximum ticks off the ground before sneaking diagonally (min range).

#### MinMaxOffGroundSneakTickDiagonal
Minimum ticks off the ground before sneaking diagonally (max range).

#### MaxMaxOffGroundSneakTickDiagonal
Maximum ticks off the ground before sneaking diagonally (max range).

### MinSneakTicks
Minimum number of ticks to sneak.

### MaxSneakTicks
Maximum number of ticks to sneak.

### NotInARow
Prevents sneaking actions from happening consecutively.

### Outliers
Enables handling of sneaking outliers (unusual ticks).

#### MinSneakTicksOutlierValue
Minimum tick count for outlier sneaks.

#### MaxSneakTicksOutlierValue
Maximum tick count for outlier sneaks.

#### MinOutlierDelay
Minimum delay before outlier sneaks.

#### MaxOutlierDelay
Maximum delay before outlier sneaks.

### MinStartSneakDistToBlock
Minimum distance from block to start sneaking.

### MaxStartSneakDistToBlock
Maximum distance from block to start sneaking.

### MinSneakBlocksForward
Minimum sneak blocks forward.

### MaxSneakBlocksForward
Maximum sneak blocks forward.

### MinSneakBlocksDiagonal
Minimum sneak blocks diagonally.

### MaxSneakBlocksDiagonal
Maximum sneak blocks diagonally.

### SneakSlowDown
Enables slowing down movement while sneaking.

### EarlySneakCalculation
Adjusts sneak calculation timing to make it more efficient.


## MovementForSneakingTrue
### ADHSMode
Controls how Anti-Directional Hits (ADHS) are handled to avoid getting caught by anti-cheat systems.
- None: No special handling for ADHS.
- ADS: Basic protection against ADHS detection.
- ADHS: Advanced protection for better anti-cheat evasion.

**ADHS = Anti-Directional Hit System**
**ADS= Advanced handling for Anti-Directional Hit detection system**

### MoveFix
Fixes movement bugs caused by the module.
- None: No fixes.
- Default: Simple fix for common problems.
- Advanced: Better fix for smoother movement.

### MoveFixIntave
Special fix for movement issues with the Intave anti-cheat system.

### SprintMode
Controls sprinting behavior.
- None: Sprinting is off.
- Legit: Sprint like a normal player.
- AllDirection: Sprint in all directions.
- AllDirectionMotion: Sprint in all directions with extra motion tweaks.

### JumpSprint
Lets you keep sprinting while jumping.

### Hover
Allows you to hover or fall slowly in the air.

### StopAtStart
Stops all movement right when the module starts.

### SafeWalkNoBlocks
Prevents you from walking off edges with no blocks underneath.

### Sneak NoBlocks
Lets you sneak even if there is no block below you.

### StopNoBlocks
Stops your movement if there is no block beneath to prevent falling.

### ReduceVelocity
Makes your speed changes smoother and more natural.

### Ignore SpeedMotion
Ignores outside speed or motion effects to keep movement steady.

### Sneak AtRotation
Automatically sneaks when you turn your view for safer movement.

### StopAtRotation
Stops your movement while you are rotating to avoid suspicious behavior.

## MovmentGodBridgeTrue
Enables God Bridging behavior — timing jumps and block placements for fast bridging without sneaking.

### DisableGodBridgeSafetyFeature
Turns off built-in safety checks that prevent failed GodBridge jumps. Not recommended unless you know what you're doing.

### MinResetGodBridgeAfterXJumps
The minimum number of jumps before the module resets the GodBridge state.

### MaxResetGodBridgeAfterXJumps
The maximum number of jumps before the module resets the GodBridge state.

### NotInARow
Prevents repeated identical jump patterns to avoid detection by anti-cheat.

### MinJumpAfterXBlocks
Minimum number of blocks placed before the next jump starts.

### MaxJumpAfterXBlocks
Maximum number of blocks placed before the next jump starts.

### MinJumpDelayAfterPlace
Minimum delay (in ms or ticks) after placing a block before jumping.

### MaxJumpDelayAfterPlace
Maximum delay (in ms or ticks) after placing a block before jumping.

### MinStartDelay
Minimum delay before the first jump when starting to GodBridge.

### MaxStartDelay
Maximum delay before the first jump when starting to GodBridge.

## MovmentMoonWalkTrue
Enables moonwalking — moving sideways while placing blocks without shifting.

### MinMoonwalkWideness
Minimum horizontal offset from the block edge while moonwalking.

### MaxMoonwalkWideness
Maximum horizontal offset from the block edge while moonwalking.

### MinMoonWalkStartDistToBlock
Minimum distance from the block when moonwalking starts.

### MaxMoonWalkStartDistToBlock
Maximum distance from the block when moonwalking starts.

### MinMoonWalkMiddle
Minimum distance used for determining the midpoint while moonwalking.

### MaxMoonWalkMiddle
Maximum distance used for determining the midpoint while moonwalking.

### NotInARow
Prevents repeated, identical moonwalk patterns to avoid anti-cheat detection.

### MinDelayToRecalculateMiddle
Minimum delay before recalculating the moonwalk middle offset.

### MaxDelayToRecalculateMiddle
Maximum delay before recalculating the moonwalk middle offset.

## SameYGroup
Keeps the player's vertical Y-level (height) consistent while bridging or walking to make movement smoother and more predictable.

### AutoJump
Automatically jumps while moving if needed to stay level or to align with block placements.

### IntaveFast2
Optimized movement logic for servers using the Intave anti-cheat system. Helps avoid flagging during SameY bridging.

### TellyBridge
Enables support for teleport bridging (Telly Bridging), where the player turns around and places blocks quickly while maintaining SameY movement.

### SafeWalk
Prevents walking off edges when bridging or moving near a drop. Especially useful for safe bridging.

### SafeWalkAir
Applies SafeWalk logic even while in mid-air (e.g., during jumps or gaps).

### SafeWalkOnlyDiagonal
Enables SafeWalk only when moving diagonally, giving more control and flexibility.

## JumpGroup
Enables jumping behavior during bridging.

### JumpOnlyWhileSpacePressed
Jumping only happens if the space key is being held. Adds manual control.

### MinJumpAfterXBlocksForward
Minimum number of blocks walked forward before jumping is triggered.

### MaxJumpAfterXBlocksForward
Maximum number of blocks walked forward before jumping is triggered.

### MinJumpAfterXBlocksDiagonal
Minimum number of blocks walked diagonally before jumping is triggered.

### MaxJumpAfterXBlocksDiagonal
Maximum number of blocks walked diagonally before jumping is triggered.

## Timer
Sets the global timer speed. A lower value slows down time-based actions, affecting game ticks. Most anti-cheats wont flag any slowdown but they will flag even a 0.1% speed up.

### TimerDrop
Temporarily lowers the timer speed after specific actions, often for anti-cheat bypass.

### MinTimerSpeed
The minimum speed the timer can drop to when triggered.

### MaxTimerSpeed
The highest timer speed the module will allow, usually used for recovery after slowdown.

## MovementMotionMultiplierTrue
### MinMotionMultiplierAirForward
Minimum forward movement multiplier while in the air. Affects speed during jumps.

### MaxMotionMultiplierAirForward
Maximum forward movement multiplier while in the air.

### NotInARow (AirForward)
Prevents repeating the same air forward multiplier value consecutively to mimic human inconsistency.

### MinMotionMultiplierAirStrafe
Minimum strafe (sideways) speed multiplier while in the air.

### MaxMotionMultiplierAirStrafe
Maximum strafe (sideways) speed multiplier while in the air.

### NotInARow (AirStrafe)
Prevents repeated strafe values to add randomness.

### MinMotionMultiplierGroundForward
Minimum forward speed multiplier while on the ground.

### MaxMotionMultiplierGroundForward
Maximum forward speed multiplier while on the ground.

### NotInARow (GroundForward)
Prevents using the same ground forward multiplier multiple times in a row.

### MinMotionMultiplierGroundStrafe
Minimum ground strafe (sideways) speed multiplier.

### MaxMotionMultiplierGroundStrafe
Maximum ground strafe (sideways) speed multiplier.

### NotInARow (GroundStrafe)
Adds variation to ground strafe movement to appear more legit.




### Legit
Builds upward realistically, mimicking normal player behavior with no suspicious movements. Safe for anti-cheat.

### Intave1
Allows tower building while moving, adapted for the Intave anti-cheat system.

### TowerWhileMoving
Lets the player build upward (tower) without stopping movement. You can walk forward or strafe while placing blocks below you — useful for smoother bridging transitions or aggressive play.

### Intave2
Similar to Intave1 but with a slightly different movement style. Also supports movement while tower building.

#### TowerWhileMoving
Lets the player build upward (tower) without stopping movement. You can walk forward or strafe while placing blocks below you — useful for smoother bridging transitions or aggressive play.

### NCP
Designed for NoCheatPlus (NCP). Allows tower building while moving, avoiding NCP flags.

#### TowerWhileMoving
Lets the player build upward (tower) without stopping movement. You can walk forward or strafe while placing blocks below you — useful for smoother bridging transitions or aggressive play.

### NCPFast
A faster version of NCP mode. Builds quicker while moving but still tuned for NCP detection.

#### TowerWhileMoving
Lets the player build upward (tower) without stopping movement. You can walk forward or strafe while placing blocks below you — useful for smoother bridging transitions or aggressive play.

### Verus
Works well with the Verus anti-cheat. Enables movement-based tower building.

#### TowerWhileMoving
Lets the player build upward (tower) without stopping movement. You can walk forward or strafe while placing blocks below you — useful for smoother bridging transitions or aggressive play.

### ConstantMotion
Tower while constantly moving forward — keeps motion smooth and uninterrupted while placing blocks upward.

#### TowerWhileMoving
Lets the player build upward (tower) without stopping movement. You can walk forward or strafe while placing blocks below you — useful for smoother bridging transitions or aggressive play.

#### ConstantMotion
Keeps the player in constant forward motion during towering, preventing stop-start movements. Makes the motion look smoother and can help bypass movement checks in anti-cheats.

### Jump
Adds jump motion during tower building with movement — looks like a player jumping while building upward.

#### TowerWhileMoving
Lets the player build upward (tower) without stopping movement. You can walk forward or strafe while placing blocks below you — useful for smoother bridging transitions or aggressive play.

#### JumpMotion
Applies a jump boost or jumping behavior during movement-based towering. The player jumps as they place blocks, mimicking how a real player might jump-tower while walking.


### SettingsForAllTowerAndSilentModes


#### SilentMode
Controls how silent block/item switching is handled:
- None: Disables silent switching entirely.
- Legit: Switches items silently in a way that mimics legitimate player behavior.
- Default: A balanced mode with decent silence and speed — standard for most use cases.
- Exploit: Uses more aggressive switching methods which may trigger silent item use in unintended ways — more detectable.

#### UseBiggestStackSilent
When enabled, always switches to the item stack with the most blocks during silent switching.

#### MinSilentStartDelay
Minimum delay (in ticks) before the silent switching process begins after activation.

#### MaxSilentStartDelay
Maximum delay (in ticks) before silent switching begins — adds randomization.

#### MinSilentSwitchDelay
Minimum delay between actual silent item switches.

#### MaxSilentSwitchDelay
Maximum delay between silent switches — allows timing variation.

#### MinStackCountToStartSwitchProcess
Minimum number of items required in a stack for the module to consider switching to it.

#### MaxStackCountToStartSwitchProcess
Maximum stack size considered for switching — useful to avoid selecting very large stacks if needed.

#### MinBackSwitchTickDelay
Minimum delay before switching back to the original item after a silent switch.

#### MaxBackSwitchTickDelay
Maximum delay before switching back to the original item.

#### DynamicBackSwitchTickDelay
When enabled, back-switch delay adapts dynamically based on context — e.g., delays more if the player is mid-action or in air.

## Visuals
### ScaffoldVisuals

### ThirdPersonMode
Shows a third-person visual to help align placements while scaffolding.

### BlockCount
Displays how many blocks are left in your inventory.

### X / Y
Sets where the BlockCount appears on the screen (X is horizontal, Y is vertical).

### Scale
Changes the size of the BlockCount display.

### BackGround
Enables a background behind the BlockCount for better visibility.

### BackGroundColor
Controls the color of the background. Works with the options below.

### Rainbow / Fade / Astolfo / ClientColor
- Rainbow: Cycles through bright rainbow colors.
- Fade: Soft fade between shades of only one color.
- Astolfo: Uses a pinkish/blueish aesthetic.
- ClientColor: Uses your selected client color setting.

### ClientColorAlpha
Sets how transparent the ClientColor is (0 = invisible, 255 = fully visible).

### RoundFactor
Rounds the corners of the BlockCount background box.

### BlockCountBlur
Adds a blur behind the BlockCount to reduce clutter.

### BlockCountShadow
Adds a shadow effect to the BlockCount text to make it easier to read.

### ESP
Highlights blocks being placed or interacted with by the scaffold.

### ESPBlur
Adds a blur effect behind ESP-highlighted blocks.

### ESPShadow
Adds a shadow around ESP-highlighted blocks to make them stand out.

### ESPColor Options (Rainbow / Fade / Astolfo / ClientColor)
Controls how the ESP blocks are colored using the selected color effect.