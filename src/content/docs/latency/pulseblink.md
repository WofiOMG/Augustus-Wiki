# PULSEBLINK
PulseBlink delays packets in bursts at set intervals, releasing multiple packets together in pulses, creating rhythmic packet bursts.

Blink simply holds all packets continuously until manually released or conditions trigger sending them all at once.

So, PulseBlink sends packets in regular timed pulses, while Blink holds them until released in one go.


**PacketDirection**
Controls which direction of packets are affected by blinking:

**OnlyIncoming**
Applies blinking only to incoming (server-to-client) packets.

**OnlyOutgoing**
Applies blinking only to outgoing (client-to-server) packets.

**Both**
Applies blinking to both incoming and outgoing packets.

**Delay Settings**
MinTickDelayBetweenLags
Minimum number of ticks to wait before starting the next blink (lag).

**MaxTickDelayBetweenLags**
Maximum number of ticks to wait before the next blink cycle.

**MinLagTicks**
Minimum number of ticks to store/delay packets during a blink.

**MaxLagTicks**
Maximum number of ticks to hold/delay packets in a blink cycle.

## Modes
Controls behavior style or logic of the blink:

**Defau**lt
Standard blinking behavior.

**DefaultCombat**
Default blinking tuned for combat scenarios.

**CombatOnly**
Only active during combat situations.

**FlushConditions**
Triggers that instantly flush all delayed packets to prevent desync or allow timely reaction:
Open, InventoryActions, Velocity, Explosion, Teleport, SprintReset, SplashPotion