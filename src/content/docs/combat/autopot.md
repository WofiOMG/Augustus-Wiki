# AUTOPOT

Automatically throws or drinks potions based on health, timing, and conditions. Used for survival, PvP, and regeneration.

**MinPitchSpeed:**
Minimum speed at which your view (pitch) adjusts when AutoPot looks down to throw a potion. Prevents slow or unnatural aim movement.

**MaxPitchSpeed:**
Maximum pitch adjustment speed for aiming downward when potting. Simulates legit player movement. If MinPitchSpeed and MaxPitchSpeed are diffrent a random value will be chosen every time.

**HealHearts:**
AutoPot activates when your health drops below the set number of hearts.

**Instant:**
When enabled, throws the potion instantly (no aim smoothing). Faster response, but flags very easy on most anti-cheats.

### When Instant is disabled you also have these options:

**MinTickDelayBeforeClick:**
Minimum delay in ticks before AutoPot performs the click action (throw/drink) after activation starts.

### MaxTickDelayBeforeClick:
Maximum delay before clicking. Adds randomness to avoid detection and simulate human reaction. 20 ticks= 1second

**MinTickDelayBetweenClick:**
Minimum delay between two AutoPot actions (if using multiple potions in sequence).

**MaxTickDelayBetweenClick:**
Maximum delay between potions thrown. Helps simulate real timing between potion throws.

**MinTickDelayAfterClick:**
Minimum delay after potion is used before the client returns to normal state (e.g., back to combat).

**MaxTickDelayAfterClick:**
Maximum delay after click. Used to randomize behavior for anti-cheat bypass.

**Hotbaronly:**
Only uses potions if they are in the hotbar. Prevents AutoPot from accessing inventory directly (safer on servers with inv checks).

**InInv:**
Allows AutoPot to access potions from inventory slots. Riskier but useful when hotbar is full or empty.

**NotWhileKillAura:**
Disables AutoPot while KillAura is active. Prevents overlap or conflicts during combat.

**Potions:**
Specifies which potion types AutoPot will use:

#### Health – Healing potions

#### Speed – Speed potions

#### Regeneration – Regen potions

#### AllPositive – Any positive effect potion (e.g., Strength, Fire Resistance)