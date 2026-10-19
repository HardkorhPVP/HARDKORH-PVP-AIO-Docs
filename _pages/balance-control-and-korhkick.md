---
title: "Balance Control & KORHKICK"
permalink: /balance/control-and-korhkick/
excerpt: "Cyclone, Root + Beam, peels and Solar Beam: how HARDKORH Balance chooses who to control, when, and with what."
toc: true
toc_label: "On this page"
---

KORHTRAP decides who to control, when, and with what. KORHKICK decides which enemy cast is worth Solar Beam. Both work for the objective [KORHTHINK]({{ '/balance/korhthink/' | relative_url }}) has set, and both leave your target alone.

## Three targets, kept separate

| Role | Who it is |
| --- | --- |
| **KILL** | Your current hostile target. Your damage goes here, and HARDKORH never changes it. |
| **CONTROL** | The player the control plan has chosen: often the enemy healer, sometimes the enemy who is bursting you. |
| **INTERRUPT** | The caster KORHKICK has chosen. |

All three can be different players at the same moment. Crowd control and Solar Beam are cast directly at their chosen unit, so your target never moves. The HUD's TARGETS row shows all three.

## How HARDKORH thinks about control

Before any crowd control, HARDKORH considers:

- **the target's role:** healer, the DPS bursting you or a teammate, or your kill target;
- **diminishing returns** on that target for that kind of control;
- **immunities:** immunity to that control, or to all damage;
- **crowd control already on the target**, so it does not overwrite or break control that is already there;
- **the current objective:** offense, defense or survival;
- **the next burst:** whether spending diminishing returns now weakens the next kill attempt;
- **range, line of sight and whether you are moving or casting**, because Cyclone and Entangling Roots are hard casts.

Crowd control is planned from Moonkin Form or caster form. A plan must hold steady for a moment before it acts (emergencies act almost at once), and a refused attempt is not retried immediately.

## Cyclone

| Purpose | When HARDKORH uses it |
| --- | --- |
| **Healer control** | On the free enemy healer in a pressure window, so your damage lands unhealed. Never when the healer is your own kill target. |
| **Defensive Cyclone** | On the enemy whose offensive cooldown is aimed at you, or at a teammate under pressure. If you are moving, an instant control on the same enemy can be used instead. |
| **Burst denial** | On an enemy who is bursting while you have no burst of your own running, in combat, with full diminishing returns. |
| **Kill-target defensive** | When your kill target is behind a major defensive outside your own burst, so the defensive runs out while that target cannot act. |
| **Heal denial** | Low value: on a low kill target you cannot finish right now while its healer is free. |
| **Between bursts** | Low value: on the free enemy healer while your Eclipse or Incarnation is about to come back. |

Every Cyclone also respects Cyclone immunity, damage immunity, existing crowd control, line of sight, range and school lockout. A Cyclone that is interrupted or broken never counts as landed, and a player who was just Cycloned is not targeted again for a few seconds.

### Midnight diminishing returns

HARDKORH reads Cyclone diminishing returns live as full, half or immune, and decides what each step is worth:

- **Full** diminishing returns are required for burst denial, kill-target defensives and the low-value uses.
- **Half** is accepted only where a shorter Cyclone still pays off: the defensive Cyclone that keeps you alive, and the enemy healer inside a strong window (your own burst, or a low kill target).
- When the enemy healer is already on half and Incarnation is ready, KORHTHINK keeps that Cyclone for the window instead of spending it early.

### Your part: stand still for Cyclone

Cyclone is a hard cast, so it only works when you cooperate. With the **Cyclone Hold-Still Cue** ON, the screen shows:

1. **CYCLONE READY / HOLD STILL**, with a sound: a Cyclone is waiting only for you to stop moving.
2. **CYCLONE / STOP MOVING**, with a second sound: the cast is starting. Moving now cancels it.

The cue appears only when the Cyclone is otherwise ready and waiting for you to stand still, never because of a cooldown, an immunity or diminishing returns. HARDKORH never cancels a Cyclone once it has started.

## Root + Beam

Solar Beam silences an area. A rooted healer cannot walk out of it.

1. **Root** the free enemy healer with Mass Entanglement, or Entangling Roots when Mass Entanglement is not available.
2. **Confirm** the root is really on the healer.
3. **Beam** the rooted healer with Solar Beam.
4. **Done** when the Beam is confirmed. The ROOT + BEAM COMPLETE notification appears only when the root, the Beam and the silence have all been seen.

If the root never appears, breaks before the Beam, or any step is refused, the setup is abandoned and that healer is left alone for a while. A healer who is root-immune, or whose damage over time would break the root, is never set up. If the healer is already rooted, HARDKORH goes straight to the Beam. While a setup is running, Solar Beam is reserved for it; only an emergency, such as crowd control cast at you, can take the Beam instead.

## Peels

When an enemy is in melee range of you and you are defending, HARDKORH peels with the first tool that fits:

1. **Incapacitating Roar** or **Mighty Bash**, whichever your talents give you;
2. **Mass Entanglement**;
3. **Typhoon**, only when you already face the enemy, because HARDKORH never turns you;
4. **Entangling Roots** last, and not when your health is critical, because it is a hard cast.

Incapacitating Roar shifts you into Bear Form. HARDKORH recognizes that Bear as its own and returns you to Moonkin when it is safe. Peels are emergency control: KORHTHINK never holds them back.

## Soothe

HARDKORH uses Soothe on an enemy that matters when the game positively identifies an Enrage effect on them.

## School lockout awareness

If you are interrupted and a spell school is locked, HARDKORH reads the lockout the game reports and does not request spells of the locked school. Where it can, it uses the other school instead: an Arcane spell when Nature is locked, or a Nature spell when Arcane is locked. When the game reports a lockout without saying which school, HARDKORH holds its spells until the lockout ends. It never invents a lockout duration.

## KORHKICK: Solar Beam

KORHKICK chooses its own interrupt target, independent of your target, and weighs:

- **the enemy cast** and what kind of spell it is;
- **how far the cast has progressed and how much is left:** never so early that it is easy to fake, never so late the Beam cannot land; channels can be silenced at any time;
- **who the cast is aimed at:** you, your healer, or another teammate;
- **the caster's role**, such as the enemy healer's heals in a pressure window;
- **the strategic state**, because while you are surviving the Beam is kept for crowd control cast at you;
- **whether the cast is proven crowd control.**

| Cast | Interrupt value |
| --- | --- |
| Crowd control aimed at you | Emergency |
| Crowd control aimed at your healer | Emergency when the fight is critical, high otherwise |
| Crowd control aimed at another teammate | High |
| The enemy healer's cast in a pressure window | High |

### Recognizing incoming crowd control

HARDKORH only classifies a cast as crowd control when a trusted source confirms it, for example:

- the game's own crowd-control spell data, used only when the cast is listed there **and** the client's spell name matches; a name-only match is never trusted;
- HARDKORH's own identification of Cyclone, which also recognizes an enemy druid's Cyclone.

Proven in live matches: **Polymorph**, **Fear** and an enemy druid's **Cyclone**. Hex and Mind Control are covered by the same trusted check. A cast that no trusted source confirms fails closed: it is not treated as crowd control, though it can still be interrupted for its other value, such as an enemy healer's heal. HARDKORH does not claim to recognize every crowd-control spell in the game.

It also knows when a Beam would be wasted. A Polymorph or Hex aimed at you while you are shapeshifted cannot affect you, so the Beam is saved. A Fear aimed at you is still silenced even when damage over time would break it early; only a true immunity skips the Beam.

## Confirmed outcomes

A success notification, such as CYCLONE LANDED or SILENCE LANDED, appears only after the effect has been seen on the enemy, never just because a spell was sent. See [KORHVISION - HUD & Cues]({{ '/balance/korhvision/' | relative_url }}).

## Not cast automatically

**Ursol's Vortex** is ground-targeted, so HARDKORH judges when it would peel and reports that in its diagnostics, but never casts it. See [Scope & Limits]({{ '/balance/scope-and-limits/' | relative_url }}).
