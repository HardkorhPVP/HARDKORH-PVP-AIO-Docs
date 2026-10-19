---
title: "Balance KORHTHINK"
permalink: /balance/korhthink/
excerpt: "The Balance strategic brain: one objective at a time, and every part of HARDKORH working toward it."
toc: true
toc_label: "On this page"
---

A rotation asks "what is the next spell?". KORHTHINK asks a different question first: **what is this moment for?**

Many times a second it reads the fight: your health and how fast it is falling, who is pressuring you, whether your healer is free, the enemy healer's state, your kill target's defensives and immunities, your Moonfire and Sunfire, Astral Power, Eclipse and Incarnation charges. From that it settles on one strategic objective. The objective is the first row of your HUD, and it decides what every other part of HARDKORH is allowed to do.

## The objectives

Survival objectives are checked first and always win. Below them, KORHTHINK picks the objective that fits the evidence. A reading HARDKORH cannot get never counts as evidence.

| Objective | When | What it changes |
| --- | --- | --- |
| **PREPARE** | The kill target cannot be pressured right now (in Cyclone or immune), your DoTs are down, or there is nothing to spend and no burst window coming. | Restore DoTs and build Astral Power. No damage into a kill target that is in Cyclone or immune. |
| **PRESSURE** | DoTs are up and a spender is ready, or a burst window is close. | Steady pressure. Low-value crowd control is saved for the coming window. |
| **CONTROL SETUP** | A healer control (Cyclone or Root + Beam) is planned or running, or clearly possible while Incarnation is ready. | Incarnation may wait briefly for the control to land. |
| **MINI GO** | An Eclipse is active. | Eclipse pressure. |
| **MAJOR GO** | Incarnation is active. | Full pressure. Only emergencies and burst-supporting control may take a global cooldown. |
| **KILL WINDOW** | Eclipse or Incarnation is running, the kill target is open, and the enemy healer is controlled or absent, or the kill target is low. | Everything goes into the kill. A KILL WINDOW cue appears on screen. |
| **DEFENSE** | Real danger: serious pressure on you, an enemy offensive cooldown aimed at you, or a peel needed. | Burst waits, offensive control waits, and Solar Beam is kept for crowd control cast at you. |
| **STABILIZE** | An emergency, or danger together with melee on you, a burst on you, your healer controlled, or a survival action already chosen. | Survival first. A waiting survival action keeps its global cooldown. A STABILIZING cue appears on screen. |
| **RECOVERY** | The moments right after danger ends, while HARDKORH's own defensive Bear is up, or at lower health with a heal ready. | A needed heal comes before preparing the next Eclipse. Burst and healer offense wait a moment. |
| **NEUTRAL** | Out of combat, no enemy player targeted, or you chose a form yourself (Cat, Travel, or a Bear you entered). | Optional low-value control is skipped. |
| **UNKNOWN** | HARDKORH cannot read your own health. | No new burst and no optional control. The rotation keeps running. |

## The objective is not cosmetic

Each objective hands a policy to the subsystems that act. This is what makes HARDKORH play as one mind instead of separate spell priorities competing for the same global cooldown.

### Burst

- Incarnation waits during DEFENSE, STABILIZE and RECOVERY, while your kill target is behind a major defensive, and briefly when a healer control is about to land.
- **Waiting is bounded.** The wait for an imminent healer control lasts only a few seconds. If the control does not happen, the burst goes ahead.
- **Charges are never wasted.** When Incarnation is about to overcap its charges, that pressure overrides the soft holds above. Hard limits still apply: no burst into an immune or Cycloned target, and none in survival danger.
- **Weak warning signs get short holds.** If the only sign of danger is an enemy offensive cooldown while you are healthy, unpressured and your healer is free, the burst waits only briefly. Real pressure keeps the hold.
- **Resources are ready when the window opens.** A ready Incarnation that is waiting pools Astral Power instead of spending it.

### Crowd control and diminishing returns

- Low-value crowd control, such as denying heals on a low target or a Cyclone to bridge two bursts, is skipped while a burst window is coming, so diminishing returns are saved for it.
- If the enemy healer is already on half diminishing returns and Incarnation is ready, that shorter Cyclone is kept for the window rather than spent early.
- During DEFENSE and STABILIZE, offensive control waits. Emergency control, a peel or a silence on crowd control cast at you, is never held back.

### Interrupts

- While you are surviving, Solar Beam is reserved for crowd control cast at you. Other high-value interrupts wait.
- Crowd control cast at your healer becomes an emergency interrupt when the fight is critical: you are defending or stabilizing, a kill window is open, your team is under pressure, or your healer is already controlled.

### Damage and recovery

- No damage goes into a kill target that is in Cyclone or immune. The HUD shows the hold. Returning to Moonkin still happens.
- In RECOVERY, a needed heal outranks preparing the next Eclipse.
- In STABILIZE, when a survival action is waiting for the global cooldown, for a refused attempt to retry or for a stun to end, a new damage spell does not take its place. The reservation is short, so the rotation never freezes.

## Worked examples

### Waiting for the healer control

Incarnation is ready, your DoTs are up, you have Astral Power, and the enemy healer is free, in range and line of sight, with full diminishing returns on Cyclone. KORHTHINK enters **CONTROL SETUP**: Incarnation waits and pools Astral Power while the Cyclone goes out. The healer is controlled, the objective becomes **KILL WINDOW**, and the burst opens with full resources.

If the Cyclone cannot happen within a few seconds, the burst goes ahead without it. If Incarnation is about to overcap its charges, it does not wait at all.

### The kill target uses a major defensive

KORHTHINK stops treating the moment as a kill window and holds the burst; the HUD names the reason. Pressure continues, and the control planner may Cyclone that target so the defensive runs out while it cannot act. Once the defensive is gone, the objective climbs back toward a kill window.

### Your healer is stunned while a melee trains you

The objective jumps to **DEFENSE**, then **STABILIZE** as your health falls. Burst and offensive control wait, Solar Beam is reserved for crowd control cast at you, and KORHSHIELD escalates: Barkskin, a peel, a heal, a defensive Bear if needed. When the pressure ends, a short **RECOVERY** puts a heal before the next Eclipse, HARDKORH returns you to Moonkin, and the objective returns to **PRESSURE**.

### A low kill target

Inside an Eclipse or Incarnation, a low kill target makes a **KILL WINDOW** even while the enemy healer is free. The window holds until that same target has been healed back up clearly, so the objective does not flicker at the edge.

## Priority between competing actions

When several parts of HARDKORH want the next global cooldown, the winner follows this order:

1. Survival actions in an emergency
2. Emergency control: peels, and a silence on crowd control cast at you
3. Defensive actions
4. High-value crowd control and interrupts
5. A prepared burst
6. Eclipse
7. Recovery heals
8. Low-value crowd control
9. Utility, such as Mark of the Wild or Remove Corruption
10. Damage

During MAJOR GO, survival always comes through, other defensives only when they are off the global cooldown or you are in danger, and recovery heals and utility wait. HARDKORH never cancels a cast you or it already started.

## Reading KORHTHINK on the HUD

The KORHTHINK row shows the objective and its reason, and names a held burst on the same row.

| The row reads | Meaning |
| --- | --- |
| `KILL WINDOW - HEALER CONTROLLED, KILL 34%` | The enemy healer is controlled; everything goes into the kill target at 34% health. |
| `KILL WINDOW - NO ENEMY HEALER, KILL 52%` | The enemy team has no healer in play. |
| <code>CONTROL SETUP - HEALER CONTROL FIRST (CYCLONE FEASIBLE) &#124; BURST HELD: CONTROL_WINDOW_IMMINENT</code> | Incarnation is waiting a few seconds for the healer Cyclone. |
| `PRESSURE - DOTS UP, SPENDER READY` | Building pressure toward the next window. |
| `PREPARE - DOTS DOWN` | Restoring Moonfire and Sunfire first. |
| `NEUTRAL - NO PLAYER KILL TARGET` | No enemy player targeted. |

Other burst-hold reasons you may see: `STABILIZE`, `DEFENSE`, `RECOVERING`, `KILL_DEFENSIVE_ACTIVE` and `SELF_STATE_UNKNOWN`. The full HUD is on [KORHVISION - HUD & Cues]({{ '/balance/korhvision/' | relative_url }}).
