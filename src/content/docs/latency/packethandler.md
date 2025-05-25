---
title: PacketHandler
---
PacketHandler is a module that modifies, delays, or hit delacancels network packets sent between the Minecraft client and server. It manages how these packets are processed to achieve effects like lag simulation, Y manipulation, packet spam control, or cheat detection avoidance. Having a better packethandler setup can give you better hitreg.

### None  
Means no delay is applied.

### MacroDelay  
Standard latency simulation.

### OtherMacroDelay  
An alternative delay mode.

### ExperimentalMacroDelay  
A test delay mode for experimental timing behavior.

### Sandwich  
Fixes delay behavior to better disguise or smooth out lag.

### RealTimeDamage  
Damage-related packets are processed immediately, without delay.

### EventToHandlePacket  
Controls when packets are handled (e.g., immediately or during event triggers).

### Vanilla  
Mimics standard Minecraft packet timing.

### Tick  
Executes once every game tick for precise control.

Delaying packets can help mimic natural network lag to avoid detection by anti-cheat systems that look for unnatural or instant actions. It can also help sync client and server data better, improving hit registration and reducing glitches caused by packet timing issues. Basically, it makes your actions appear more "human" and smooth to the server.

All packets that you can abort or delay:

Incoming Packets (Server → Client)

---

### Chat

* **S02PacketChat** – Receives chat messages from the server.

---

### Time & World

* **S03PacketTimeUpdate** – Updates world time (day/night cycle).
* **S21PacketChunkData** – Sends chunk data to load terrain.
* **S22PacketMultiBlockChange** – Multiple block changes in one area.
* **S23PacketBlockChange** – A single block update.
* **S24PacketBlockAction** – Updates block state (e.g., note block play).
* **S25PacketBlockBreakAnim** – Shows block breaking animation.
* **S26PacketMapChunkBulk** – Sends multiple chunks at once.
* **S27PacketExplosion** – Triggers explosion effects.
* **S44PacketWorldBorder** – Updates the world border.
* **S2BPacketChangeGameState** – Changes game state (e.g., rain starts, win screen).

---

### Entity & Movement

* **S04PacketEntityEquipment** – Updates entity equipment (e.g., armor).
* **S06PacketUpdateHealth** – Updates player health.
* **S07PacketRespawn** – Handles respawn mechanics.
* **S08PacketPlayerPosLook** – Teleports and rotates the player.
* **S09PacketHeldItemChange** – Changes currently held item.
* **S0APacketUseBed** – Entity uses a bed.
* **S0BPacketAnimation** – Plays animation (e.g., swing arm).
* **S0CPacketSpawnPlayer** – Spawns another player entity.
* **S0DPacketCollectItem** – Item pickup animation.
* **S0EPacketSpawnObject** – Spawns entities like boats, arrows.
* **S0FPacketSpawnMob** – Spawns mobs (zombies, etc).
* **S10PacketSpawnPainting** – Spawns a painting.
* **S11PacketSpawnExperienceOrb** – Spawns XP orbs.
* **S12PacketEntityVelocity** – Sets entity velocity.
* **S13PacketDestroyEntities** – Removes entities.
* **S14PacketEntity** – Basic entity update.
* **S15PacketEntityRelMove** – Moves entity relatively.
* **S16PacketEntityLook** – Updates entity rotation only.
* **S17PacketEntityLookMove** – Moves and rotates entity.
* **S18PacketEntityTeleport** – Teleports entity.
* **S19PacketEntityHeadLook** – Rotates entity head.
* **S1APacketEntityStatus** – Entity status update (e.g., hurt).
* **S1BPacketEntityAttach** – Attaches entities (e.g., mount).
* **S1CPacketEntityMetadata** – Updates entity data (e.g., name).
* **S1DPacketEntityEffect** – Applies a potion effect.
* **S1EPacketRemoveEntityEffect** – Removes a potion effect.
* **S20PacketEntityProperties** – Sends attribute data (e.g., speed).
* **S49PacketUpdateEntityNBT** – Sends NBT data of an entity.

---

### Inventory & GUI

* **S2DPacketOpenWindow** – Opens GUI (e.g., chest, furnace).
* **S2EPacketCloseWindow** – Closes GUI.
* **S2FPacketSetSlot** – Sets item in inventory slot.
* **S30PacketWindowItems** – Sends entire inventory contents.
* **S31PacketWindowProperty** – Updates GUI property (e.g., furnace progress).
* **S32PacketConfirmTransaction** – Confirms inventory actions.
* **S33PacketUpdateSign** – Updates a sign’s text.
* **S35PacketUpdateTileEntity** – Sends NBT update to tile entities.
* **S36PacketSignEditorOpen** – Opens sign editing GUI.

---

### Scoreboard & Tablist

* **S37PacketStatistics** – Sends game statistics.
* **S38PacketPlayerListItem** – Updates player tab list.
* **S3BPacketScoreboardObjective** – Scoreboard objective updates.
* **S3CPacketUpdateScore** – Updates individual scores.
* **S3DPacketDisplayScoreboard** – Selects active scoreboard.
* **S3EPacketTeams** – Updates scoreboard teams.
* **S47PacketPlayerListHeaderFooter** – Header/footer in tab list.

---

### Sound & Visual Effects

* **S28PacketEffect** – Plays block effects (e.g., door open).
* **S29PacketSoundEffect** – Plays global sound.
* **S2APacketParticles** – Spawns particles.
* **S2CPacketSpawnGlobalEntity** – Spawns lightning bolt.
* **S45PacketTitle** – Displays title/subtitle on screen.

---

### Misc / Other

* **S3APacketTabComplete** – Tab-completion suggestions.
* **S3FPacketCustomPayload** – Custom plugin data.
* **S40PacketDisconnect** – Disconnects the player.
* **S41PacketServerDifficulty** – Updates game difficulty.
* **S42PacketCombatEvent** – Sends combat-related event (e.g., death).
* **S43PacketCamera** – Changes camera target.
* **S46PacketSetCompressionLevel** – Sets compression level.
* **S48PacketResourcePackSend** – Sends a resource pack.

---

## Outgoing Packets (Client → Server)

---

### Keep Alive

* **C00PacketKeepAlive** – Responds to keep-alive ping.

---

### Chat & Commands

* **C01PacketChatMessage** – Sends a chat message.
* **C14PacketTabComplete** – Requests tab completions.

---

### Movement & Actions

* **C02PacketUseEntity** – Attacks or interacts with entity.
* **C03PacketPlayer** – Base movement packet.
* **C04PacketPlayerPosition** – Sends position only.
* **C05PacketPlayerLook** – Sends rotation only.
* **C06PacketPlayerPosLook** – Sends position and rotation.
* **C07PacketPlayerDigging** – Starts/stops block breaking.
* **C08PacketPlayerBlockPlacement** – Places a block or interacts.
* **C09PacketHeldItemChange** – Changes selected hotbar slot.
* **C0APacketAnimation** – Triggers animation (e.g., swing arm).
* **C0BPacketEntityAction** – Sneak, sprint, jump, etc.

---

### Inventory & GUI

* **C0CPacketClickWindow** – Clicks inside an inventory.
* **C0DPacketCloseWindow** – Closes inventory.
* **C0EPacketClickWindow** – (Duplicate, possibly mistaken).
* **C11PacketEnchantItem** – Applies an enchantment.
* **C12PacketUpdateSign** – Sends text to server sign.

---

### Player Status & Settings

* **C13PacketPlayerAbilities** – Updates abilities (fly, invulnerable).
* **C15PacketClientSettings** – Client settings (e.g., language).
* **C16PacketClientStatus** – Client status like respawn.

---

### Custom & Miscellaneous

* **C17PacketCustomPayload** – Plugin channel communication.
* **C18PacketSpectate** – Spectate another player.
* **C19PacketResourcePackStatus** – Resource pack loading status.
* **CAnimateHandPacket** – Triggers hand animation (possibly mod-specific or renamed version).

