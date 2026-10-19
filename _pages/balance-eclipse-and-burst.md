---
title: "Balance Eclipse & Burst"
permalink: /balance/eclipse-and-burst/
excerpt: "Astral Power, the Eclipse cycle and charge-aware Incarnation: how HARDKORH builds pressure and turns it into a kill window."
toc: true
toc_label: "On this page"
---

Eclipse and Incarnation never happen by accident. HARDKORH prepares for them, enters them on purpose, and times them with crowd control and with your survival.

## How Eclipse works in Midnight

In the current Balance design, Eclipse is one activatable ability with charges:

- Your spell book shows it as **Solar Eclipse**. Casting **Starfire** turns it into **Lunar Eclipse**; casting **Wrath** turns it back into **Solar Eclipse**.
- Solar and Lunar are two faces of the same learned action. They share one set of charges, and the game decides which face it offers right now.

HARDKORH works with that model directly:

- **It looks before it acts.** Before activating anything, HARDKORH reads which Eclipse the game is offering at that moment. It activates only the Eclipse it positively sees offered, never a guess.
- **It reads, never assumes.** Charges, recharge time, usability and cooldowns come from your client while you play. No charge count or duration is hard-coded.
- **It knows what really happened.** After an activation, HARDKORH records which Eclipse the game actually entered, so the next decision builds on what happened, not on what was asked for.

## The Eclipse cycle

<ol class="hk-flow">
  <li><span>PREPARE</span></li>
  <li><span>SELECT</span></li>
  <li><span>ENTER</span></li>
  <li><span>PRESSURE</span></li>
  <li><span>EXIT</span></li>
  <li><span>PREPARE NEXT</span></li>
</ol>

| Step | What HARDKORH does |
| --- | --- |
| **Prepare** | Restores or refreshes Moonfire and Sunfire and builds Astral Power for an opening spender. Preparation is bounded: it never waits more than a few seconds, and never while the Eclipse charges are full. |
| **Select** | If the Eclipse it wants is not the one on offer, it casts the spell that changes it: Starfire for Lunar, Wrath for Solar. While one Eclipse is being prepared, it never casts the builder that would switch the selection away. |
| **Enter** | Activates the Eclipse the game is offering, as soon as it reads ready. |
| **Pressure** | Spends Astral Power and uses the empowered builder of that Eclipse, such as Wrath inside Solar. A DoT that has dropped off comes before a paid Starsurge; a free Starsurge still comes first. Healthy DoTs are not refreshed early. |
| **Exit and prepare next** | When the Eclipse ends, the cycle starts again for the other Eclipse. |

HARDKORH alternates between Solar and Lunar, starting from the Eclipse you were last really in; at the start of a session it takes whichever is on offer. It never stalls the rotation waiting for a perfect Eclipse:

- if the selection has not changed after a couple of selector casts, it enters the Eclipse that is on offer;
- if the game keeps refusing the Eclipse request, it backs off for a moment and keeps casting (the HUD shows the block and its reason).

### Total Eclipse

Sometimes the game enters Solar and Lunar together; the HUD shows **ECLIPSE BOTH**. HARDKORH treats that as a successful entry of the Eclipse it asked for and continues the alternation from there: for example Lunar, then both, then Solar next. When Incarnation itself puts you in both Eclipses, HARDKORH knows no Eclipse charge was spent and does not count it as its own entry.

## Astral Power

- **The real maximum.** Your Astral Power maximum is read live, never assumed.
- **No overcapping.** When the room left is smaller than the cost of a Starsurge, HARDKORH spends. The HUD marks the ASTRAL POWER row CAP RISK or AT CAP.
- **Pooling with a purpose.** Astral Power is held back only when an Eclipse or Incarnation can really start soon: ready now, or its next charge almost back. Otherwise it is spent normally.
- **Free and instant opportunities.** When the game reports that Starsurge costs nothing, or that a spell casts instantly, HARDKORH takes that opportunity first.

## Incarnation: charge-aware burst

Incarnation: Chosen of Elune is HARDKORH Balance's major cooldown. Its readiness comes from the charges the game reports, never from a fixed timer, so HARDKORH knows whether a cast spends your last charge or one that is about to come back anyway.

HARDKORH starts Incarnation when the window is prepared:

- your target is an enemy player who is not immune, not in Cyclone and not in breakable crowd control;
- Moonfire and Sunfire are up and you can afford a spender, or one is free;
- no Solar or Lunar Eclipse with more than a few seconds left is running, because Incarnation brings both Eclipses with it;

or when charge pressure demands it: the charges are full, or the next charge is almost back, so waiting would waste one.

It never starts Incarnation while you are in survival danger, out of combat, or without an enemy player as your target, and it never cancels an Incarnation that is running.

On top of that, [KORHTHINK]({{ '/balance/korhthink/' | relative_url }}) holds the burst while you defend, stabilize or recover, while your kill target is behind a major defensive, and for a few seconds while a healer control is about to land. Charge pressure overrides these soft holds. A ready Incarnation that is waiting pools Astral Power, so the window opens with resources.

Inside Incarnation (MAJOR GO), HARDKORH quickly restores any DoT that dropped off, free spenders first, and keeps the pressure on. Only emergencies and burst-supporting control interrupt it.

## Burst thinking

<ol class="hk-flow hk-flow--burst">
  <li><span>PREPARE</span></li>
  <li><span>CONTROL SETUP</span></li>
  <li><span>HEALER CONTROL</span></li>
  <li><span>INCARNATION / ECLIPSE</span></li>
  <li class="hk-flow__goal"><span>KILL WINDOW</span></li>
</ol>

HARDKORH reasons about your DoTs, Astral Power, Eclipse, Incarnation charges and the risk of overcapping them, whether the enemy healer is controlled, whether your kill target is immune or behind a defensive, and your own survival. A burst that would go into an immune target, into a Cyclone, or while you are fighting for your life waits. A burst that would waste a charge does not.

## On the HUD

| Row | Reads |
| --- | --- |
| **ASTRAL POWER** | Current / maximum, with CAP RISK or AT CAP when spending is due. |
| **ECLIPSE** | SOLAR, LUNAR or BOTH with the time left, or NONE. |
| **ECLIPSE ACTION** | The Eclipse the game is offering right now and its state: READY with charges, RECHARGING with the time left, or BLOCKED with the reason. |
| **ECLIPSE NEXT** | The Eclipse HARDKORH is preparing and its plan, for example READY or WAIT FOR CHARGE. |
| **MOONFIRE / SUNFIRE** | UP with the time left and REFRESH WINDOW when a refresh is due, DOWN, or NO TARGET. |
| **OPPORTUNITY** | FREE STARSURGE or an INSTANT cast when the game offers one. |
| **INCARNATION** | READY with charges and the burst decision, RECHARGING, or ACTIVE with the time left. |

Moonfire and Sunfire are timed from what HARDKORH observed itself applying to each target, and refreshed late in their duration so nothing is clipped. When HARDKORH cannot tell whether a DoT is up, it treats it as unknown rather than guessing either way.
