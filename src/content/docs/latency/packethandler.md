# PACKETHANDLER
PacketHandler is a module that intercepts, modifies, delays, or hit delacancels network packets sent between the Minecraft client and server. It manages how these packets are processed to achieve effects like lag simulation, y manipulation, packet spam control, or cheat detection avoidance. Having a better packethandler setup can give you better hitreg.

## MacroDelay Modes set how packets are delayed:

**None**
Means no delay,

**MacroDelay**
Is standard latency simulation.

**OtherMacroDelay**
Is an alternative delay.

**ExperimentalMacroDelay**
Is a new test delay.

**Sandwich**
Fixes delays for better disguise.

**RealTimeDamage**
Means damage packets are processed immediately.

**EventToHandlePacket**
Decides when packet handling runs.

**Vanilla**
For standard Minecraft events.

**Tick**
Runs every game tick for precise control.

Delaying packets can help mimic natural network lag to avoid detection by anti-cheat systems that look for unnatural or instant actions. It can also help sync client and server data better, improving hit registration and reducing glitches caused by packet timing issues. Basically, it makes your actions appear more "human" and smooth to the server.

All packets that you can abort or delay:

Incoming Packets (Server → Client)

#### Keep Alive
S00PacketKeepAlive

#### Chat
S02PacketChat

#### Time & World
S03PacketTimeUpdate

S21PacketChunkData

S22PacketMultiBlockChange

S23PacketBlockChange

S24PacketBlockAction

S25PacketBlockBreakAnim

S26PacketMapChunkBulk

S27PacketExplosion

S44PacketWorldBorder

S2BPacketChangeGameState

#### Entity & Movement
S04PacketEntityEquipment

S06PacketUpdateHealth

S07PacketRespawn

S08PacketPlayerPosLook

S09PacketHeldItemChange

S0APacketUseBed

S0BPacketAnimation

S0CPacketSpawnPlayer

S0DPacketCollectItem

S0EPacketSpawnObject

S0FPacketSpawnMob

S10PacketSpawnPainting

S11PacketSpawnExperienceOrb

S12PacketEntityVelocity

S13PacketDestroyEntities

S14PacketEntity

S15PacketEntityRelMove

S16PacketEntityLook

S17PacketEntityLookMove

S18PacketEntityTeleport

S19PacketEntityHeadLook

S1APacketEntityStatus

S1BPacketEntityAttach

S1CPacketEntityMetadata

S1DPacketEntityEffect

S1EPacketRemoveEntityEffect

S20PacketEntityProperties

S49PacketUpdateEntityNBT

#### Inventory & GUI
S2DPacketOpenWindow

S2EPacketCloseWindow

S2FPacketSetSlot

S30PacketWindowItems

S31PacketWindowProperty

S32PacketConfirmTransaction

S33PacketUpdateSign

S35PacketUpdateTileEntity

S36PacketSignEditorOpen

#### Scoreboard & Tablist
S37PacketStatistics

S38PacketPlayerListItem

S3BPacketScoreboardObjective

S3CPacketUpdateScore

S3DPacketDisplayScoreboard

S3EPacketTeams

S47PacketPlayerListHeaderFooter

#### Sound & Visual Effects
S28PacketEffect

S29PacketSoundEffect

S2APacketParticles

S2CPacketSpawnGlobalEntity

S45PacketTitle

#### Misc / Other
S3APacketTabComplete

S3FPacketCustomPayload

S40PacketDisconnect

S41PacketServerDifficulty

S42PacketCombatEvent

S43PacketCamera

S46PacketSetCompressionLevel

S48PacketResourcePackSend

#### Outgoing Packets (Client → Server)
#### Keep Alive
C00PacketKeepAlive

#### Chat & Commands
C01PacketChatMessage

C14PacketTabComplete

#### Movement & Actions
C02PacketUseEntity

C03PacketPlayer

C04PacketPlayerPosition

C05PacketPlayerLook

C06PacketPlayerPosLook

C07PacketPlayerDigging

C08PacketPlayerBlockPlacement

C09PacketHeldItemChange

C0APacketAnimation

C0BPacketEntityAction

#### Inventory & GUI
C0CPacketClickWindow

C0DPacketCloseWindow

C0EPacketClickWindow

C11PacketEnchantItem

C12PacketUpdateSign

#### Player Status & Settings
C13PacketPlayerAbilities

C15PacketClientSettings

C16PacketClientStatus

#### Custom & Miscellaneous
C17PacketCustomPayload

C18PacketSpectate

C19PacketResourcePackStatus

CAnimateHandPacket

