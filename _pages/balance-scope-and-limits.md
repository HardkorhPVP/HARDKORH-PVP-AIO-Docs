---
title: "Balance Scope & Limits"
permalink: /balance/scope-and-limits/
excerpt: "What HARDKORH Balance is built for, what it deliberately leaves to you, and how it behaves when it cannot be sure."
---

HARDKORH Balance is purpose-built PvP intelligence. It does what it can prove it does well, and it says plainly where it stops.

## Built for PvP

The strategy, crowd control, interrupt and defensive intelligence is designed for Arena, Solo Shuffle, Battlegrounds and world PvP against enemy players.

Outside PvP, the normal combat abilities still work where they apply:

- the rotation, the Eclipse cycle and DoT upkeep run on your current hostile target, including NPCs and target dummies;
- defensives and heals still react to your health and how fast it is falling, but the threat readings behind them (enemy burst, melee pressure, healer state) come from enemy players only; Mark of the Wild is still kept up;
- Incarnation is used automatically only when your target is an enemy player, so on NPCs and dummies it stays yours;
- crowd control and Solar Beam are planned around enemy players and stay idle otherwise.

There is no dungeon or raid logic: no boss mechanics, no affix handling and no multi-target encounter play. A target dummy is still a good place to check your HUD and the basic rotation.

## Always yours

HARDKORH never:

- moves your character or navigates;
- turns you to face a target (Typhoon is used only when you already face one);
- changes your WoW target or focus;
- cancels a cast that is in progress;
- cancels a form you chose: Cat Form, Travel Form or a Bear Form you entered.

## Deliberately not automated

Some abilities stay with you because HARDKORH cannot yet use them with the same proven reliability as the rest. That is a choice, not an oversight:

| Ability | Why it stays manual |
| --- | --- |
| **Starfall** | Its value depends on multi-target positioning that HARDKORH does not yet judge with proven intelligence. |
| **Force of Nature** | Used only if the game reports it as a targeted spell. When the game reports it as ground-targeted, the HUD shows READY - GROUND TARGETED - NOT AUTOMATED and it stays yours. |
| **Ursol's Vortex** | Ground-targeted, with no verified ground-target route. HARDKORH judges when it would peel and reports that in diagnostics, but never casts it. |
| **Fury of Elune** | Not part of the validated Balance build. |
| **Dispelling teammates** | Remove Corruption is used on you only. Teammate dispels wait for a proven way to cast on a friendly player. |

Trinkets and movement abilities are always your call.

## When HARDKORH cannot be sure

HARDKORH fails closed. When something cannot be read, it does not guess:

- an ability whose readiness, charges or cost cannot be read is not used;
- a crowd-control cast that no trusted source confirms is not treated as crowd control;
- a defensive or heal is not used when your health, the effect type or the ability state cannot be read;
- if HARDKORH cannot read your own health, it starts no new burst and no optional crowd control, while the rotation keeps running;
- if the execution layer cannot be proven safe at load, the HUD reads UNAVAILABLE and nothing is cast.

The result is a HARDKORH that sometimes waits when a guess might have worked, and never acts on information it does not have.

<div class="notice--warning" markdown="1">
**Please read.** HARDKORH is third-party automation software for the Project Sylvanas platform. It is not made, endorsed or approved by Blizzard Entertainment. Using third-party automation may violate the World of Warcraft Terms of Use and can lead to action against your account. No rating, win rate or outcome is guaranteed.
</div>
