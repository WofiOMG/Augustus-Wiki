# PING
Temporarily stores (chokes) movement packets and releases them all at once to simulate lag or desync. This allows you basically teleport on most servers.

**PacketDirection**
Controls which packets are intercepted:

**OnlyIncoming:**
 Only blocks incoming server packets.

**OnlyOutgoing:**
 Only blocks outgoing player packets.

**AutoDisable**
Automatically disables the module after X ticks. Example: 7 ticks: you will move freely for 350ms while appearing to other people "bugged" and after 7 ticks you will be teleported for your oponents.

**DisableOnAttack**
Disables Blink when you attack an entity (optional for legit appearance).

**DisableKillAura**
Disables Blink if KillAura is enabled. Helps prevent detection during combat. Interacting with other players wont work while using blink anyways.