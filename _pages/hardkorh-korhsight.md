---
title: "KORHSIGHT - Targeting"
permalink: /hardkorh/korhsight/
excerpt: "One validated KILL target that keeps your pressure where you put it."
---

KORHSIGHT picks and keeps the **KILL** target: the enemy player your damage goes to. It never changes your WoW target or focus.

## The KILL target

With **Option C Live Targeting** ON (a session-only switch in the KORHSIGHT card, turned on once per session for PvP):

- your own valid enemy player target always wins;
- with no target, the Project Sylvanas target selector's player can be used;
- the KILL survives brief target loss.

With Option C OFF, damage follows your current WoW target, including NPCs and dummies. Turn it OFF on target dummies and in PvE.

## Pressure and continuity

- The KILL row shows exactly who is taking your damage.
- The KILL does not flicker to whoever is closest; it stays until you switch target, the player dies, or it is lost for more than a moment.
- To switch pressure, simply target the new enemy player. Your switch always wins.

## KILL vs CONTROL

KILL is your damage target. **CONTROL** is the crowd-control target: with CC Healer ON it is the enemy healer. If the HUD shows CONTROL NONE (NO HEALER), the game has no validated healer and hard CC holds.

The two can be different players at the same time. KORHSIGHT owns the KILL and keeps your damage there; [KORHTRAP]({{ '/hardkorh/korhtrap/' | relative_url }}) owns the CONTROL target and plans crowd control on it. Your damage does not move to the healer because it is the CONTROL target.

{% include hk-figure.html src="/assets/images/screenshots/11-kill-control-example.png" alt="Arena combat: the HUD shows a KILL target at 21% health and a separate enemy healer as CONTROL, with ACTION MOONFIRE (Lunar Inspiration) and BURST SETUP" w="1915" h="705" caption="KILL and CONTROL at the same time: damage stays on the KILL target while the enemy healer is tracked as a separate CONTROL target." %}

## Reading it on the HUD

| Row | What to look for |
| --- | --- |
| **KILL** | Name, HEALER or TANK tag when known, health % and distance. Flags such as DEAD, IMMUNE, CYCLONED or CC when they apply. |
| **CONTROL** | "= KILL" when it is the same unit; otherwise the healer with its current CC and time left, or FREE. |
| **HOLD** | Why damage is held, for example KILL IMMUNE or KILL CC PROTECTED. A held KILL target in Cyclone or breakable CC is deliberate: switch to another enemy if you want to keep pressure. |
