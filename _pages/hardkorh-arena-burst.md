---
title: "Arena Burst"
permalink: /hardkorh/arena-burst/
excerpt: "Coordinated kill windows: Incarnation or Berserk while the enemy healer is controlled."
toc: true
toc_label: "On this page"
---

The major cooldown is Incarnation when you have it learned, otherwise Berserk. In Arena, HARDKORH spends it only in an authorized kill window, and only while **Arena Burst** is ON.

## Turning it on

| Control | Behavior |
| --- | --- |
| **Arena Burst** switch (BURST card, this session only) | OFF: in Arena the major cooldown is never used by the kill-window logic. ON: a stable kill window with the enemy healer controlled may trigger the major cooldown. It returns to OFF on every reload. |
| **Arena Burst Key** (keybind, saved) | Turns Arena Burst ON or OFF with one key press, with the menu open or closed. Purple = ON, gray = OFF. The key is saved; Arena Burst itself still returns to OFF on every reload. |

Arena Burst needs **CC Healer ON**, because only then does HARDKORH track the enemy healer. It does not affect burst in Battlegrounds or open world, Tiger's Fury, or Feral Frenzy.

## Reading the BURST row in Arena

| BURST reads | Meaning |
| --- | --- |
| **OFF** | Arena Burst is off. |
| **SETUP** | A kill window is building. |
| **HOLD** | The window is not ready yet; the reason is shown. |
| **GO** | The window is authorized and the major cooldown fires. |
| **ACTIVE** | The major burst window is active. |

## When a kill window is authorized

With Arena Burst ON, a window is authorized only when:

- every visible enemy healer is under real crowd control (Cyclone, incapacitate, stun, disorient, fear or silence, from anyone; roots do not count) with at least about two seconds left;
- the KILL is a non-healer enemy player within about 8 yards, not immune, not in Cyclone or breakable CC;
- your Rake and Rip are up and not about to expire, and you have hit the KILL in the last few seconds;
- you are in Cat, healthy enough, free of crowd control, not casting and not in an emergency defensive;
- the major cooldown is ready and the window holds for a moment.

One major cooldown is spent per window. Windows without a healer, or where the KILL is the healer, are not authorized. Tiger's Fury and Feral Frenzy run normally in every case. Burst is always held during a defensive stage, and into a target that is immune, in Cyclone, in breakable CC or behind heavy damage reduction.

{% include hk-figure.html src="/assets/images/screenshots/18-arena-burst-active.png" alt="Arena combat: BURST reads ACTIVE, the CONTROL healer is incapacitated and ACTION FEROCIOUS BITE continues on the KILL target at 23% health" w="1670" h="621" caption="BURST ACTIVE: the enemy healer is controlled on the CONTROL row and HARDKORH keeps the pressure on the KILL target during the active burst window." %}

<div class="notice--warning" markdown="1">
**No-healer games**

Arena Burst only trusts healer-controlled windows. Against a team without a healer, the Arena kill-window logic never spends the major cooldown. If you want to burst in those games, use Incarnation or Berserk yourself.
</div>

## Burst outside Arena

| Environment | When burst fires |
| --- | --- |
| **Battleground** | In Cat and in combat with Rake and Rip up on the target. It waits for Tiger's Fury when Tiger's Fury is ready. |
| **Open-world PvP** | In Cat and in combat with Rake and Rip up on the target. |
| **Outside PvP** | On cooldown in Cat while in combat. |
