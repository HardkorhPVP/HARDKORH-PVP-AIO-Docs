---
title: "KORHTRAP - Crowd Control"
permalink: /hardkorh/korhtrap/
excerpt: "Healer control, Incapacitating Roar and the four-stage Cyclone, and how your movement makes it work."
toc: true
toc_label: "On this page"
---

KORHTRAP picks one **CONTROL** target and asks whether hard crowd control on it is useful and safe right now. Controlling the healer is what turns pressure into kills: KORHTRAP aims Incapacitating Roar and Cyclone at the healer while your damage stays on the KILL.

<div class="notice--info" markdown="1">
**Turn these on each session**

**CC Healer**, **Incapacitating Roar Live** and **Cyclone Live** are session-only switches in the KORHTRAP card. They start OFF after every reload; turn all three ON before you queue.
</div>

## Who gets controlled

- **CC Healer ON:** the CONTROL target is the nearest validated enemy healer, rescanned during combat. A player whose role is unknown is never treated as a healer. With no healer, crowd control holds; it never falls back to a DPS.
- **CC Healer OFF:** the CONTROL target is your KILL target.

## The Cyclone, step by step

Cyclone is a hard cast on the enemy healer, so it only works when you cooperate: plant your feet when the cue asks. The cue appears in the middle of the screen, separate from the HUD window.

### <span class="hk-stage">1</span> CYCLONE READY / HOLD STILL

HARDKORH has found a Cyclone opportunity on the CONTROL healer and asks you to stay put. A short sound plays with it. **Stop moving now** so the cast can begin.

{% include hk-figure.html src="/assets/images/screenshots/12-cyclone-ready.png" alt="The CYCLONE READY / HOLD STILL cue above an enemy mage, with the HUD showing a KILL target and the enemy healer as CONTROL" w="1920" h="782" caption="Step 1: CYCLONE READY / HOLD STILL." %}

### <span class="hk-stage">2</span> CYCLONE / STOP MOVING

The cast is starting right now, with a second sound. **Do not move**: moving interrupts the cast.

{% include hk-figure.html src="/assets/images/screenshots/13-cyclone-stop-moving.png" alt="The CYCLONE / STOP MOVING cue in the middle of an Arena fight" w="1139" h="647" caption="Step 2: CYCLONE / STOP MOVING." %}

### <span class="hk-stage">3</span> The cast is in progress

The HUD confirms the hard cast: **ACTION** reads CYCLONE CASTING and **HOLD** reads CYCLONE CAST IN PROGRESS. Damage waits while the cast runs, and HARDKORH never cancels it once it is committed.

{% include hk-figure.html src="/assets/images/screenshots/14-cyclone-casting.png" alt="The STOP MOVING cue with the HUD showing ACTION CYCLONE CASTING and HOLD CYCLONE CAST IN PROGRESS, and the Cyclone cast bar under the player frame" w="1890" h="857" caption="Step 3: ACTION CYCLONE CASTING, HOLD CYCLONE CAST IN PROGRESS." %}

### <span class="hk-stage">4</span> CYCLONE confirmed

A green CYCLONE check confirms the cast landed. The CONTROL row now shows the healer as controlled (DISORIENTED), and HARDKORH is back on the KILL target.

{% include hk-figure.html src="/assets/images/screenshots/15-cyclone-confirmed.png" alt="A green CYCLONE check mark above the target, with the HUD showing the enemy healer DISORIENTED on the CONTROL row and ACTION SHRED on the KILL target" w="1995" h="923" caption="Step 4: CYCLONE confirmed; the healer is controlled and pressure resumes." %}

## Cyclone rules

- Healer only, never your KILL target, within about 25 yards and in line of sight.
- It needs you **standing still** and not casting, because it is a hard cast.
- It is skipped when the healer is immune to Cyclone or damage, when disorient diminishing returns are too far along, or during urgent defensives, an interrupt or a burst window.
- It is not repeated on the same healer within a few seconds of an accepted Cyclone.
- It yields to Incapacitating Roar when Roar is available with equal or better diminishing returns.
- While the cast runs, everything else waits except Barkskin, Survival Instincts and Healthstone. HARDKORH never cancels the cast.

## Incapacitating Roar

- An instant area incapacitate on the CONTROL target, within about 10 yards.
- It needs the target confirmed not immune and diminishing returns fresh enough.
- It is skipped when the target is already controlled for more than a moment, or when your own bleeds would break it.
- It yields to your defensives and to Skull Bash.
- With CC Healer OFF it lands on your KILL target, and HARDKORH then holds damage so the incapacitate is not broken.

## Diminishing returns and immunity

Diminishing returns halve CC duration with each application in the same category. KORHTRAP tracks DR per target and category and skips CC that would be too short to matter. Immunities are checked before every cast. An unknown immunity state blocks Roar rather than risking a wasted cast.

## Control sequencing

CC is planned around the rest of the fight. Survival actions come first, Skull Bash outranks Roar, and Cyclone waits while you are in an urgent defensive stage. Burst waits for control. Your damage holds on a KILL target that is in Cyclone or breakable CC.

## Positioning: your part of the plan

- Stand within Roar range of the healer for an incapacitate.
- Keep line of sight on the healer and plant your feet for Cyclone.
- Move only when you must. The HOLD STILL cue is your signal.

**Why poor movement loses CC.** Every step during the Cyclone cast cancels it. Constant strafing keeps the window from ever opening, and fighting behind a pillar from the healer removes line of sight. When CC "never happens", movement and range are the first things to check.

<div class="notice--warning" markdown="1">
**Avoid fighting the system**

- Do not cast your own Cyclone at the same time; let the cue lead.
- Do not trinket or move out of the cast without a reason.
- If you want a specific manual CC, press your Enable Plugin key first, then turn it back on.
</div>
