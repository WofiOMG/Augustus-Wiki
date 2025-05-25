---
title: AimAssist
---

### MinPreAimRange:  
How close the target needs to be for aim to start locking on. Lower = aim starts sooner.

### MaxPreAimRange:  
How far away aim assist works. Higher = lock-on from further away. Diffrent values shows randomness.

### Mode: Stable, Experimental  
- **Stable**: Basic, safe version with reliable behavior.  
- **Experimental**: May feel snappier or more aggressive but less predictable. 

### ImproveYourAimInput  
Boosts how your mouse input is used. Makes small movements smoother and more precise.

---
### Mode: Experimental

### Strength:  
Controls how strong the experimental aim assist is. Higher values = more aggressive snapping or correction.

### FasterMouseMovement:  
If true, allows aim assist to react quicker to fast mouse movements. Helps keep up when you flick or turn fast.

---
### Mode: Stable

#### OwnHorizontalRotationMultiplier:  
How much your left/right mouse movement affects rotation. Higher = faster turn speed.

#### OwnVerticalRotationMultiplier:  
Same as above but for up/down (pitch) movement.

#### HorizontalAssistMultiplier:  
How much the aim helps side-to-side. Boost this if you're missing left/right.

#### VerticalAssistMultiplier:  
Helps you stay on target up/down. Useful if targets jump or crouch.

#### AutoAim  
Turns on automatic aiming. Will aim at targets without manual input if not using Click setting.

#### MinHorizontalSpeed:  
The slowest side-to-side speed auto-aim will move at.

#### MaxHorizontalSpeed:  
The fastest auto-aim is allowed to move side-to-side.

#### MinVerticalSpeed:  
Slowest up/down speed auto-aim uses.

#### MaxVerticalSpeed:  
Fastest up/down speed auto-aim uses.

#### HorizontalSmoothness:  
Controls how "soft" the aim glides left/right. Higher = less snappy.

#### VerticalSmoothness:  
Same thing but for up/down aiming.

#### SmoothEarly:  
If true, it starts smoothing at the beginning of the aim move instead of snapping first.

#### NoRotationFovMode: 2D, 3  
- **2D**: Only checks horizontal FOV.  
- **3**: Uses full 3D box for smarter detection, better with vertical targets or flying ones.

#### NoRotationHorizontal:  
Width of the area where aim doesn't rotate the view. Good for looking legit.

#### NoRotationVertical:  
Height of that same no-rotate box.

#### HorizontalBoxSize:  
How wide the total no-rotation zone is around your crosshair.

#### RandomizationStrength:  
How much randomness is added to aim. Higher = more human-looking, less snappy.

#### RandomizeInNoRotationFovs:  
If true, adds randomness even when you’re inside the no-rotation zone.

### HorizontalFov:  
How far left/right your aim will look for targets.

### VerticalFov:  
How far up/down your aim will look for targets.

### Click:  
AimAssist will only rotate player when clicking attack button. Use AutoClicker module if you dont like clicking.

### DiggingCheck:  
If true, disables aim when breaking blocks. Keeps you from snapping while mining.

### SingleTarget:  
If on, only focuses one target at a time. Stops switching mid-fight.

### Targets: Player, Mob, Animal, Villager, ArmorStand, Invisible, Dead, Teammates  
What kind of entities the aim system can lock onto. Turn off stuff you don’t want to hit.

### Weapons: Axes, Fists, Rest, Rods, Sticks, Swords  
Lets you choose which weapons activate the AimAssist when all conditions are meet. 
