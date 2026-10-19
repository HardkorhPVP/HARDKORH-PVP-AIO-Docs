---
title: "Balance KORHVISION"
permalink: /balance/korhvision/
excerpt: "The Balance combat HUD, the KILL WINDOW and STABILIZING cues, and notifications for control that really landed."
toc: true
toc_label: "On this page"
---

KORHVISION shows what HARDKORH Balance is thinking and doing. It is display only: it never casts, targets, moves or cancels anything, and combat is identical with every option on this page off.

## The Balance HUD

The Balance HUD is its own on-screen window, with the HARDKORH header and a state badge:

| Badge | Meaning |
| --- | --- |
| <span class="hk-pill hk-pill--live">LIVE</span> | Balance Execution is ON and HARDKORH is acting. |
| <span class="hk-pill hk-pill--disabled">DISABLED</span> | Balance Execution is OFF. Nothing is cast. |
| <span class="hk-pill hk-pill--amber">DRY RUN</span> | An engineering setting is on: HARDKORH decides but never casts. Not for normal play. |
| <span class="hk-pill hk-pill--disabled">UNAVAILABLE</span> | HARDKORH could not prove its execution layer safe at load, so it will not cast. Reload; if it persists, contact support. |

The window shows while **Balance Combat HUD** is ON (the default). **Balance Diagnostics** adds an engineering section for support.

## The rows

| Row | Shows |
| --- | --- |
| **KORHTHINK** | The current objective and its reason, and a held burst with its reason. See [KORHTHINK]({{ '/balance/korhthink/' | relative_url }}). |
| **MODE** | What the damage side is doing, for example BUILD, SPEND, POOL, OVERCAP, DOT_REFRESH, ECLIPSE_PREPARE, ECLIPSE_SELECTOR, ECLIPSE_ENTER, MINI_GO, MAJOR_GO or HOLD. |
| **ACTION** | The action being cast. If the game refused it, ACTION shows BLOCKED or FAILED, or RETRYING while it is retried. |
| **REASON** | Why that action was chosen, or why it failed. |
| **PVP** | OFFENSE, DEFENSE or NEUTRAL, with the reason. |
| **TARGETS** | KILL, CONTROL and INTERRUPT: three roles that can be three different players. |
| **CONTROL PLAN** | The crowd control HARDKORH is planning and what it is waiting for, such as WAIT STILL. |
| **DEFENSE** | NORMAL, PRESSURED, DANGER or EMERGENCY, with the reason. |
| **DEFENSIVE ACTION** | The survival action chosen right now, or NONE. |
| **HEALER** | Your own healer: FREE, CONTROLLED or NONE. |
| **BEAR** | OFF, HARDKORH's own Bear with its reason, or MANUAL for a Bear you entered. |
| **ASTRAL POWER** | Current / maximum, with CAP RISK or AT CAP. |
| **SCHOOL LOCK** | NONE, or the locked school and the time left. |
| **ECLIPSE** | SOLAR, LUNAR or BOTH with the time left, or NONE. |
| **ECLIPSE ACTION** | The Eclipse the game is offering and whether it can be entered. |
| **ECLIPSE NEXT** | The next Eclipse HARDKORH is preparing, and its plan. |
| **MOONFIRE / SUNFIRE** | Your own DoT on the target: UP with the time left, REFRESH WINDOW, DOWN, or NO TARGET. |
| **OPPORTUNITY** | FREE STARSURGE or an INSTANT cast when the game offers one. |
| **FORCE OF NATURE** | Its state. READY - GROUND TARGETED - NOT AUTOMATED means it is yours to cast. |
| **INCARNATION** | READY with charges and the burst decision, RECHARGING, or ACTIVE with the time left. |
| **CAST** | Shown while HARDKORH's own hard cast is in progress. |

Each row's colour only helps you read it at a glance; the text always states the condition. Green is good or active, amber is preparing or waiting, red is danger or a failure, purple is information, gray is off or unknown.

## Strategic cues

Two short on-screen cues mark the turning points of a fight. They appear only when KORHTHINK actually changes to that objective.

| Cue | Meaning |
| --- | --- |
| **KILL WINDOW** (cyan) | The objective has become a kill window: your burst is running and the enemy healer is controlled or absent, or your kill target is low. |
| **STABILIZING** (red) | The objective has become STABILIZE: survival comes first right now. |

Turn them off with **Strategic Cues** in [Balance Settings]({{ '/balance/settings/' | relative_url }}).

## Control success notifications

A short notification confirms crowd control that HARDKORH cast and **saw land**:

| Notification | Shown when |
| --- | --- |
| **CYCLONE LANDED** | The Cyclone cast completed and the Cyclone is seen on the enemy. |
| **SILENCE LANDED** | Solar Beam is confirmed and the silence is seen on the enemy. |
| **STUN LANDED** | Mighty Bash is confirmed and a stun is seen on the enemy. |
| **ROOT LANDED** | Entangling Roots completed, or Mass Entanglement is confirmed, and the root is seen on the enemy. |
| **KNOCKBACK LANDED** | Typhoon is confirmed and the knockback is seen on the enemy. |
| **ROOT + BEAM COMPLETE** | The root was seen, the Beam was confirmed and the silence was seen: the whole setup worked. |

A notification never appears for a spell that was only sent, was interrupted, failed, or was not seen landing. Each shows briefly, a few can stack, and repeats are suppressed. They have no sound. Turn them off with **Control Success Notifications**.

## Cyclone hold-still cue

Before a HARDKORH Cyclone, a cue in the middle of the screen asks you to cooperate:

1. **CYCLONE READY / HOLD STILL**, with a sound: the Cyclone is waiting only for you to stop moving.
2. **CYCLONE / STOP MOVING**, with a second sound: the cast is starting. Moving now cancels it.

The cue shows while Balance Execution is LIVE. It never changes what is cast. Turn it off with **Cyclone Hold-Still Cue**. More on the [control page]({{ '/balance/control-and-korhkick/#your-part-stand-still-for-cyclone' | relative_url }}).

## Diagnostics

**Balance Diagnostics** adds an engineering section to the same window: identities read from your spell book, executor results, control tools and arbitration, school lockout, Incarnation charges, and KORHTHINK's inputs and policies. It is for support; leave it off for play. **Balance Diagnostic Logging** writes the same story to a log file; see [Balance Settings]({{ '/balance/settings/' | relative_url }}).
