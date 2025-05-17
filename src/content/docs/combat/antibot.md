# ANTIBOT

**AntiBot** module filters and ignores bots, NPCs, and fake players such as shopkeepers or anti-cheat decoys.

Mode:
**IsInTabList**
Ignores entities that are not in the tab list. Real players appear in tab; bots and NPCs usually don’t.

**Advanced**
Uses multiple detection checks combined. Helps catch more complex or disguised bots.

**Hypixel**
Activates custom checks for Hypixel. Ignores shopkeepers, NPCs, and anti-cheat bots unique to that server.

**Intave**
Detects bots used by the Intave anti-cheat system. Looks for fake movement and behavior.

**NullTeam**
Flags entities that have no team assigned. Real players usually have one (even if invisible).

**IllegalPitch**
Detects bots with invalid pitch (vertical rotation), such as values beyond normal limits.

**Ticks Existed**
Flags entities that have existed for only a few ticks. Bots are often freshly spawned.

**NegativeHealth**
Detects bots with negative health, which is impossible for real players.

**ZeroPing**
Flags entities showing 0ms ping – usually fake, server-side bots or NPCs.

**InvalidEntity ID**
Detects entities with invalid or out-of-range entity IDs.

**InvalidName**
Flags weird or malformed names. Often used by bots or NPCs.

**Never OnGround**
Flags entities that are always airborne or never touch the ground.

**Swinged**
Detects if an entity has never swung its arm (no attacks or interactions). Bots usually don't swing.

**ItemInHand**
Flags entities with no valid item held. Real players usually hold an item.

**Armor**
Detects bots with no or unusual armor setups.

**Sound**
Flags entities that produce no normal player sounds (footsteps, damage sounds).

<div style="border-left: 5px solid #E94B35; background-color: #FDECEA; padding: 15px; color: #B22222; font-family: Arial, sans-serif; border-radius: 8px; max-width: 600px; box-shadow: 0 2px 5px rgba(233,75,53,0.3);">
  <strong style="font-size: 18px; display: flex; align-items: center; margin-bottom: 8px;">
    ⚠️ Warning: AntiBot Module Recommended
  </strong>
  <p style="font-size: 16px; line-height: 1.4;">
    Not using AntiBot modules can lead to faster bans on servers that use fake players to detect hacks like KillAura.  
    Protect yourself by enabling AntiBot features.
  </p>
</div>
