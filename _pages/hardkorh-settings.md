---
title: "Settings"
permalink: /hardkorh/settings/
excerpt: "The HARDKORH settings page, card by card, with the recommended values."
toc: true
toc_label: "Settings cards"
---

The settings page follows one order from top to bottom, one section card at a time. Switches show ON or OFF directly; hover any option for a one-line description, and right-click it to reset it to its default. All read-only status lives at the very bottom, in SYSTEM STATUS and SUPPORT DIAGNOSTICS.

{% include hk-figure.html src="/assets/images/screenshots/01-hardkorh-settings-overview.png" alt="The HARDKORH PVP AIO v1.0.0 settings page open in the Project Sylvanas menu, with the KORHVISION HUD reading LIVE on the left" w="1574" h="1304" caption="The HARDKORH PVP AIO v1.0.0 settings page with the KORHVISION HUD." %}

## HardkorhPVP recommended settings

Rows marked **VALIDATED** match the validated HARDKORH configuration used in live Arena and Solo Shuffle play. **DEFAULT** rows are the shipped defaults, recommended as a starting value. **RECOMMENDED** marks a HardkorhPVP recommendation for a session-only control.

| Setting | Recommended | Basis |
| --- | --- | --- |
| Enable Plugin | ON when you want automation | VALIDATED |
| Combat HUD | ON | VALIDATED |
| Diagnostics Panel | OFF | DEFAULT |
| HUD Left / Top / Scale | 1 / 28 / 100, then drag the HUD where you want it | DEFAULT |
| Cyclone Cast Cue | ON | VALIDATED |
| Cyclone Cast Sound | ON | VALIDATED |
| Option C Live Targeting | ON in PvP; OFF on dummies and in PvE | VALIDATED |
| CC Healer | ON | VALIDATED |
| Incapacitating Roar Live | ON | VALIDATED |
| Cyclone Live | ON | VALIDATED |
| Arena Burst | ON | VALIDATED |
| Strength of the Wild Live | ON (each session) | RECOMMENDED |
| Interrupt At Cast | 70% | DEFAULT |
| Diagnostic File Logging | ON | VALIDATED |
| Verbose PvP Events | OFF | DEFAULT |
| Decision Engine (ADVANCED) | ON (never change) | DEFAULT |
| Dry Run (ADVANCED) | OFF (never change) | DEFAULT |

## GENERAL OPTIONS

The first card. A short build line at the bottom identifies the installed version for support: **HARDKORH PVP AIO v1.0.0 - Feral M6.6**.

| Option | What it does | Recommended / default |
| --- | --- | --- |
| **Enable Plugin** (switch, saved) | The master switch. ON = LIVE: HARDKORH runs everything in this guide, with no arm step. OFF stops every decision and cast, and clears any pending request. It does not affect the Combat HUD, which stays visible and reads DISABLED, the keys, or any saved setting. | ON whenever you want automation. Default OFF. |
| **Enable Plugin Key** (keybind, saved) | Turns Enable Plugin on or off with one key press. Purple = enabled, gray = disabled. | Bind a key you can reach in combat. Default unbound. |

## KORHVISION

Display only: combat is identical with every option in this card OFF.

| Option | What it does | Recommended / default |
| --- | --- | --- |
| **Combat HUD** (switch, saved) | Shows or hides the compact [KORHVISION HUD]({{ '/hardkorh/korhvision/' | relative_url }}) window. It stays visible while the plugin is disabled. Hide it for screenshots or recordings. | ON. Default ON. |
| **Combat HUD Key** (keybind, saved) | Shows or hides the Combat HUD with one key press. | Optional. Default unbound. |
| **Diagnostics Panel** (switch, saved) | Adds the dense technical DIAGNOSTICS section at the bottom of the HUD window. It draws only while the Combat HUD is visible. | OFF for play; turn it on when support asks. Default OFF. |
| **Diagnostics Panel Key** (keybind, saved) | Shows or hides the Diagnostics Panel with one key press. | Optional. Default unbound. |
| **HUD Left** (slider 0-100%, saved) | Horizontal position of the HUD window's left edge, as a percentage of the screen width. Dragging the window updates it. | Default 1. Easiest: drag the HUD. |
| **HUD Top** (slider 0-100%, saved) | Vertical position of the HUD window's top edge, as a percentage of the screen height. | Default 28. Easiest: drag the HUD. |
| **HUD Scale** (slider 60-160%, saved) | Text size step: below 90% compact, 90-129% standard, 130% and above large. The text always uses the client's native window fonts. | Default 100. |
| **Cyclone Cast Cue** (switch, saved) | The two-stage on-screen Cyclone warning: HOLD STILL, then STOP MOVING. It never delays or cancels a cast. | ON. Default ON. |
| **Cyclone Cast Sound** (switch, saved) | Two short sounds per HARDKORH Cyclone: one when the window develops, one when the cast starts. | ON. Default ON. |

{% include hk-figure.html src="/assets/images/screenshots/06-korhvision-settings.png" alt="The KORHVISION settings card: Combat HUD, Combat HUD Key, Diagnostics Panel and its key, HUD Left, HUD Top, HUD Scale, Cyclone Cast Cue and Cyclone Cast Sound" w="562" h="373" class="hk-figure--small" caption="The KORHVISION card." %}

## KORHSIGHT

| Option | What it does | Recommended |
| --- | --- | --- |
| **Option C Live Targeting** (switch, this session only) | Chooses what HARDKORH's damage follows. OFF (after every reload): damage follows your current WoW target, including NPCs and dummies. ON: damage follows KORHSIGHT's sticky KILL target, a validated enemy player that stays put instead of flickering between targets. It never changes your WoW target, and Skull Bash always interrupts your WoW target. | ON in Arena, Shuffle and Battlegrounds. OFF on target dummies and in PvE. |

More: [KORHSIGHT - Targeting]({{ '/hardkorh/korhsight/' | relative_url }}).

## KORHTRAP

| Option | What it does | Recommended |
| --- | --- | --- |
| **CC Healer** (switch, this session only) | ON: Incapacitating Roar and Cyclone are reserved for a validated enemy healer. With no healer, CC holds; it never falls back to a DPS. OFF: the plan follows your KILL target. Cyclone and Arena Burst both need CC Healer ON. | ON. |
| **Incapacitating Roar Live** (switch, this session only) | OFF: Roar is only planned. ON: a fully checked Roar may be cast on the CONTROL target. Enable Plugin must also be ON. | ON. |
| **Cyclone Live** (switch, this session only) | OFF: Cyclone is only planned. ON: a fully checked Cyclone may be cast on the enemy healer. It is never cast on your KILL target, and it yields to Roar when Roar is the better option. Stand still when the cue says HOLD STILL. | ON, together with CC Healer ON. |

{% include hk-figure.html src="/assets/images/screenshots/07-korhsight-korhtrap-settings.png" alt="The KORHSIGHT card with Option C Live Targeting and the KORHTRAP card with CC Healer, Incapacitating Roar Live and Cyclone Live, all switched ON" w="556" h="266" class="hk-figure--small" caption="KORHSIGHT and KORHTRAP, set up for PvP." %}

More: [KORHTRAP - Crowd Control]({{ '/hardkorh/korhtrap/' | relative_url }}).

## BURST

| Option | What it does | Recommended / default |
| --- | --- | --- |
| **Arena Burst** (switch, this session only) | OFF: in Arena the major cooldown is never used by the kill-window logic. ON: a stable kill window with the enemy healer controlled may trigger the major cooldown. It returns to OFF on every reload. It does not affect burst in Battlegrounds or open world, Tiger's Fury, or Feral Frenzy. | ON. Turn it on once per session before Arena or Shuffle. |
| **Arena Burst Key** (keybind, saved) | Turns Arena Burst ON or OFF with one key press, with the menu open or closed. Purple = ON, gray = OFF. The key is saved; Arena Burst itself still returns to OFF on every reload. | Optional. Default unbound. |

More: [Arena Burst]({{ '/hardkorh/arena-burst/' | relative_url }}).

## KORHSHIELD

Defensives are fully automatic and have no settings ([KORHSHIELD - Defensives]({{ '/hardkorh/korhshield/' | relative_url }})).

| Option | What it does | Recommended |
| --- | --- | --- |
| **Strength of the Wild Live** (switch, this session only) | Allows Strength of the Wild in a Bear Form that HARDKORH entered itself. OFF: it is not used, and the normal Bear rotation (Mangle, Thrash, Swipe) runs. ON: with a KILL target in reach, unprotected, the spell ready and no survival action pending, it is cast ahead of Mangle. Survival actions and Skull Bash always come first. | ON. Turn it on once per session. |

## KORHKICK

| Option | What it does | Recommended |
| --- | --- | --- |
| **Interrupt At Cast** (slider 10-100%, saved) | How far an interruptible enemy cast must have progressed before Skull Bash fires. Lower interrupts earlier, which is more reliable against short casts but easier for the enemy to fake. Higher interrupts later. The interrupted unit is always your current WoW target. | 70% (default). |

{% include hk-figure.html src="/assets/images/screenshots/08-korhshield-korhkick-settings.png" alt="The KORHSHIELD card with Strength of the Wild Live and the KORHKICK card with the Interrupt At Cast slider" w="561" h="194" class="hk-figure--small" caption="KORHSHIELD and KORHKICK. Strength of the Wild Live is shown OFF, as it is after every reload; the recommendation is ON." %}

KORHUSE has no card: Healthstone, Mark of the Wild and Predatory Swiftness Regrowth are automatic and have no settings.

## LOGGING & SUPPORT

| Option | What it does | Recommended / default |
| --- | --- | --- |
| **Diagnostic File Logging** (switch, saved) | Writes a diagnostic log file while the plugin is enabled. Combat is not affected. | ON. Default ON. |
| **Verbose PvP Events** (switch, saved) | Adds detailed spell-cast event records to the log. It only makes the log larger. | OFF; turn it on only when support asks. Default OFF. |

## ADVANCED

<div class="notice--warning" markdown="1">
**Leave these at their defaults**

The ADVANCED card is for development and support. For normal play: **Decision Engine ON, Dry Run OFF**.
</div>

| Option | Default and effect |
| --- | --- |
| **Decision Engine** (switch, saved, engineering) | ON. OFF stops every automated decision; the HUD reads DECISION OFF. |
| **Dry Run (decide, never cast)** (switch, saved, engineering) | OFF. ON makes HARDKORH decide without casting anything; the HUD reads DRY RUN in amber. |
| **Runtime Probe Key** (keybind, saved, engineering) | Unbound. A status indicator for support. It gates nothing and changes nothing. |

## SYSTEM STATUS and SUPPORT DIAGNOSTICS

**SYSTEM STATUS** sits below all settings: a short read-only summary of the HARDKORH state (LIVE, DISABLED, DRY RUN or DECISION OFF), Environment, Current Action, KILL, CONTROL, Defensive State and Burst State. The live rows read "-" while the plugin is disabled.

**SUPPORT DIAGNOSTICS** is the last card on the page. Its sections start collapsed; expand one only when support asks: Player Keybind Diagnostics, HARDKORHKIT Composition, Targeting Diagnostics, Control Diagnostics, Defensive Diagnostics, Burst Diagnostics, Executor Diagnostics and Raw Telemetry.

{% include hk-figure.html src="/assets/images/screenshots/09-logging-support-diagnostics.png" alt="The bottom of the settings page: LOGGING & SUPPORT, the ADVANCED card, SYSTEM STATUS rows and the collapsed SUPPORT DIAGNOSTICS subsections" w="557" h="784" class="hk-figure--small" caption="LOGGING & SUPPORT, ADVANCED, SYSTEM STATUS and SUPPORT DIAGNOSTICS at the bottom of the page." %}

## Automatic abilities without a card

| Ability | What HARDKORH does |
| --- | --- |
| **Mark of the Wild** | Recast when it is missing, out of combat. Requires caster or Cat form, and you not mounted, casting, stealthed or in owned Bear. |
| **Skull Bash** | Interrupts an interruptible cast of your WoW target once it passes Interrupt At Cast %. Usable from Cat or Bear. Focus is not used. |
| **Wild Charge** | Closes the gap toward the KILL target when it is outside melee range and the charge is castable. It yields to an imminent burst. |
| **Typhoon** | From an owned defensive Bear when the KILL target is in range and in front of you. HARDKORH never turns you to face it. |
| **Heart of the Wild** | In an owned Bear, when it is ready. The exact spell is identified from your client at login. |
| **Strength of the Wild** | In an owned Bear with Strength of the Wild Live ON, ahead of Mangle when everything lines up. |
| **Ursol's Vortex** | Not cast. Good Vortex moments are shown on the HUD as VORTEX SHADOW so you can cast it yourself. |
| **Travel Form, Dash, Stampeding Roar, Prowl** | Not cast. These stay manual. |
