---
title: "Balance Settings"
permalink: /balance/settings/
excerpt: "The HARDKORH PVP AIO - BALANCE settings page: every option, its default and the recommended value."
toc: true
toc_label: "On this page"
---

On a Balance Druid, open the Project Sylvanas menu and then **HARDKORH PVP AIO - BALANCE**. All Balance options live in one card, **BALANCE - PVP DAMAGE + CONTROL**. Balance settings are separate from the Feral settings and are saved between sessions.

## Recommended settings

| Setting | Recommended | Default |
| --- | --- | --- |
| Balance Execution | ON when you want automation | OFF |
| Balance Execution Key | A key you can reach in combat | Unbound |
| Balance Dry Run | OFF (never change) | OFF |
| Balance Combat HUD | ON | ON |
| Balance Diagnostics | OFF; turn on when support asks | OFF |
| Balance Diagnostic Logging | ON | ON |
| Strategic Cues | ON | ON |
| Control Success Notifications | ON | ON |
| Cyclone Hold-Still Cue | ON | ON |

## The options

| Option | What it does |
| --- | --- |
| **Balance Execution** (switch) | The master switch. ON: HARDKORH runs everything in the Balance guide: the rotation, Eclipse and Incarnation on your current hostile target; crowd control, Solar Beam and Soothe on the unit it chooses; and survival on you. OFF: nothing is cast. A Bear Form you entered yourself is never cancelled. |
| **Balance Execution Key** (keybind) | Turns Balance Execution on or off with one key press, with the menu open or closed. The key itself is saved; it never acts as a second switch. |
| **Balance Dry Run** (switch, engineering) | Decides and validates every action but never casts. The HUD reads DRY RUN. For verification only. |
| **Balance Combat HUD** (switch) | Shows the [Balance HUD]({{ '/balance/korhvision/' | relative_url }}): the KORHTHINK objective, the action and its reason, PvP mode, the kill, control and interrupt targets, the control plan, defense, Astral Power, school lockout, Eclipse, DoTs and Incarnation. |
| **Balance Diagnostics** (switch) | Adds the engineering section to the HUD window: spell identities, executor results, control tools, arbitration, school lockout and Incarnation charges. Leave it off for normal play. |
| **Balance Diagnostic Logging** (switch) | Writes Balance decisions and observations to a diagnostic log file. The Feral log is not touched. |
| **Strategic Cues** (switch) | A short on-screen cue when KORHTHINK's objective changes to KILL WINDOW or STABILIZING. Display only. |
| **Control Success Notifications** (switch) | A short on-screen confirmation when a HARDKORH crowd control is seen on the enemy: CYCLONE LANDED, SILENCE LANDED, STUN LANDED, ROOT LANDED, KNOCKBACK LANDED, ROOT + BEAM COMPLETE. Never shown for a cast that was only sent, interrupted, failed or not seen landing. Display only. |
| **Cyclone Hold-Still Cue** (switch) | Before a HARDKORH Cyclone, CYCLONE READY / HOLD STILL with a sound; when the cast starts, CYCLONE / STOP MOVING with a sound. Display and sound only; it never changes what is cast. |

A line at the bottom of the card summarizes the scope: no movement, facing or target changes; Starfall and Ursol's Vortex stay manual; Feral is unchanged.

## One switch, saved

Balance Execution is the one deliberate safety boundary for Balance. There are no separate per-session LIVE switches: crowd control, interrupts, defensives and burst all run under Balance Execution. It is OFF on a new install. Like every Balance option it is saved, so it is still ON after a reload if you left it ON.

Your Balance Execution Key is the fastest way to take over: one press stops everything, another press resumes.

## Logs for support

1. Keep **Balance Diagnostic Logging** ON.
2. Reproduce the problem.
3. Before you reload, copy `scripts_log/hardkorh/balance_pvp.log` from your Project Sylvanas folder. The file holds the latest session only, so a reload starts it over.

Report problems on [Discord](https://discord.gg/sv2WNwk2WZ) with the time, what you expected, a screenshot of the HUD and the log. See [Troubleshooting]({{ '/support/troubleshooting/' | relative_url }}).
