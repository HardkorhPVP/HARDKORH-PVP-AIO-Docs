---
title: "KORHVISION"
permalink: /hardkorh/korhvision/
excerpt: "The compact combat HUD: what HARDKORH sees and does, at a glance."
toc: true
toc_label: "On this page"
---

**Feral Druid.** For the Balance HUD and its cues, see [Balance KORHVISION]({{ '/balance/korhvision/' | relative_url }}).

The Combat HUD is a compact on-screen window. It shows what HARDKORH sees and does. It is display only: it never casts, targets, moves or cancels anything, and combat is identical with it hidden.

{% include hk-figure.html src="/assets/images/screenshots/04-korhvision-live.png" alt="The KORHVISION HUD reading LIVE out of combat: KILL, CONTROL and ACTION NONE, BURST READY, DEFENSIVE NONE 100%" w="364" h="256" class="hk-figure--small" caption="The Combat HUD in LIVE operation before a fight: nothing to act on yet, burst ready." %}

## The master state

The HUD is a native Project Sylvanas window: a dark panel with a purple border and a purple header, in the client's own sharp window fonts. The master state sits in a small pill at the right of the HARDKORH header, always as text.

| Badge | Meaning |
| --- | --- |
| <span class="hk-pill hk-pill--live">LIVE</span> | Enable Plugin is ON and HARDKORH is acting. |
| <span class="hk-pill hk-pill--disabled">DISABLED</span> | Enable Plugin is OFF. Nothing is decided or cast. The HUD shows a single row: STATE PLUGIN DISABLED - NO AUTOMATION. |
| <span class="hk-pill hk-pill--amber">DRY RUN</span> | An engineering override is on: HARDKORH decides but never casts. Not for normal play. |
| <span class="hk-pill hk-pill--info">DECISION OFF</span> | An engineering override has switched the decision engine off. Not for normal play. |

{% include hk-figure.html src="/assets/images/screenshots/02-korhvision-disabled.png" alt="The KORHVISION HUD with a red DISABLED pill and the single STATE cell PLUGIN DISABLED - NO AUTOMATION" w="377" h="94" class="hk-figure--small" caption="DISABLED: Enable Plugin is OFF and nothing is decided or cast." %}

## The rows

| Row | Shows |
| --- | --- |
| **KILL** | The damage target: name, HEALER or TANK tag when known, health % and distance. Flags such as DEAD, IMMUNE, CYCLONED or CC appear when they apply. NONE when there is no valid target. |
| **CONTROL** | The crowd-control target. "= KILL" when it is the same unit. A healer shows with its current CC and time left, or FREE. With CC Healer ON and no healer found it reads NONE (NO HEALER). |
| **ACTION** | What HARDKORH is doing now: a cast and its result (CAST, OK, REFUSED, PENDING), CYCLONE CASTING, or HOLD. |
| **HOLD** | Shown only when damage is held, with the reason. Examples: STUNNED, CYCLONE CAST IN PROGRESS, NOT IN CAT FORM, DAMAGE HELD, SURVIVAL INSTINCTS ACTIVE, CRITICAL HP, NO KILL, KILL IMMUNE, KILL CC PROTECTED, FRIENDLY TARGET. |
| **BURST** | Major cooldown state. In Arena: OFF (Arena Burst is off), SETUP, GO, HOLD with a reason, or ACTIVE. Elsewhere: READY, GO, SETUP, HOLD, COOLDOWN or ACTIVE. |
| **DEFENSIVE** | The current defensive stage and your health %. |
| **BEAR** | OWNED (HARDKORH entered Bear Form itself), REQUESTED, RECOVERY (TO CAT), MANUAL (UNOWNED) or NONE. |
| **CC** | Cyclone and Incapacitating Roar status side by side: CASTING, CAST, READY, OFF, or a short reason. |
| **UTILITY** | Heart of the Wild, Typhoon and Strength of the Wild in owned Bear; CHARGE when the KILL target is out of melee; VORTEX SHADOW when Ursol's Vortex would fit (it is shown, never cast). |
| **KICK** | Shown only when an interrupt is relevant: the enemy spell and its progress, KICKING, or CD while Skull Bash is on cooldown. |

## Status colours

Each row is a label with a status cell. The text always says the state; the colour only helps you read it at a glance:

- **green**: LIVE, ON, ready or cast;
- **red**: DISABLED, critical health or a strong defensive (for example BARKSKIN);
- **amber**: setting up, waiting, or DRY RUN;
- **purple or white**: information, such as the KILL and CONTROL targets;
- **gray**: OFF, unknown, none or not applicable.

The cells only show state. Clicking them does nothing.

## Moving and sizing the HUD

- **Move it** by dragging the window. HARDKORH saves the position in HUD Left and HUD Top, so it opens in the same place after a reload. Moving those sliders moves the window too.
- **Size**: HUD Scale picks one of three text sizes: below 90% compact, 90-129% standard (default 100), 130% and above large. The window fits its content; it cannot be resized by hand.
- **Show or hide** it with the Combat HUD switch or the Combat HUD Key. The window has no close button.

## Diagnostics Panel

The Diagnostics Panel is an extra DIAGNOSTICS section at the bottom of the same HUD window (the window grows wider and taller) with technical values for troubleshooting and support. It covers target source, control internals, executor result and reason, pending request, burst, defense, CC and utility details. It is off by default and draws only while the Combat HUD is visible. Turn it on when support asks for a screenshot.

{% include hk-figure.html src="/assets/images/screenshots/05-korhvision-diagnostics.png" alt="The KORHVISION HUD with the Diagnostics Panel: the status cells and, below them, the DIAGNOSTICS section with technical rows" w="647" h="666" class="hk-figure--small" caption="The HUD with the Diagnostics Panel." %}

## Cyclone cue and sound

For HARDKORH's own Cyclone only, a cue appears in the middle of the screen, separate from the HUD window, and walks you through the cast in four steps: CYCLONE READY / HOLD STILL, CYCLONE / STOP MOVING, the cast in progress, and CYCLONE confirmed. Two short sounds play with the first two steps. The full sequence, with real match screenshots, is on the [KORHTRAP]({{ '/hardkorh/korhtrap/' | relative_url }}) page.
