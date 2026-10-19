---
title: "Troubleshooting"
permalink: /support/troubleshooting/
excerpt: "Fixes for the common questions, how to collect logs, and where to get help."
toc: true
toc_label: "Problems"
---

<p><a class="btn btn--primary btn--large" href="https://discord.gg/sv2WNwk2WZ" rel="noopener">JOIN DISCORD</a></p>

Questions and help: **🆘・support**. Reproducible bugs: **🐛・bug-fixes**. Keep Project Sylvanas updated to the latest available version before reporting a problem.

## The plugin appears disabled

- Check SYSTEM STATUS at the bottom of the HARDKORH page, and the HUD badge. <span class="hk-pill hk-pill--disabled">DISABLED</span> means Enable Plugin is OFF; turn it on with the switch in GENERAL OPTIONS or its key.
- After a settings reset, Enable Plugin is OFF again by design.
- If the HARDKORH PVP AIO entry is missing completely, check that you are on a Druid in Feral or Balance specialization. On Balance the entry is **HARDKORH PVP AIO - BALANCE**.

## Balance is not casting

- Check the Balance HUD badge. <span class="hk-pill hk-pill--disabled">DISABLED</span> means Balance Execution is OFF: turn it on with its switch or the Balance Execution Key.
- <span class="hk-pill hk-pill--amber">DRY RUN</span> means Balance Dry Run is ON: turn it OFF.
- <span class="hk-pill hk-pill--disabled">UNAVAILABLE</span> means HARDKORH could not prove its execution layer safe at load and will not cast. Reload; if it stays, report it with the log.
- Read the ACTION and REASON rows: a refused cast shows BLOCKED or FAILED with the game's reason.
- HARDKORH does not shift you out of Cat Form, Travel Form or a Bear Form you entered yourself. Return to Moonkin or caster form.
- Target a hostile unit; your current hostile target receives your damage. See [Balance Settings]({{ '/balance/settings/' | relative_url }}).

## The HUD is hidden

- Check that Combat HUD is ON in the KORHVISION card, or press the Combat HUD Key.
- Check HUD Left and HUD Top: values near 100 push the panel off screen. Try the defaults 1 and 28.
- The Diagnostics Panel only draws inside a visible HUD.

## A keybind is assigned but does not respond

- Keys are yours to assign: click the keybind field on the HARDKORH page and press the key you want. See [Keybinds]({{ '/getting-started/keybinds/' | relative_url }}).
- Scroll to SUPPORT DIAGNOSTICS and expand Player Keybind Diagnostics. Each row shows the bind's state, last toggle source, key code and press count.
- If the press count does not rise when you press the key, the key is not reaching the plugin. Reassign it, or pick a key that is not used elsewhere.
- If the purple / gray highlight disagrees with the setting, the setting is still correct. Report the bind's "raw" row, including its `sync=` value.

## Dry Run or Decision Off was turned on by accident

SYSTEM STATUS and the HUD badge read <span class="hk-pill hk-pill--amber">DRY RUN</span> in amber, and nothing is cast. In the ADVANCED card, turn **Dry Run OFF**. The same applies to **DECISION OFF**: turn **Decision Engine** back ON. For normal play: Decision Engine ON, Dry Run OFF.

## HARDKORH is not attacking a dummy or an NPC

Option C Live Targeting only attacks enemy players. Turn it OFF, and enter Cat Form yourself; outside PvP HARDKORH does not shift for you. See [PvE]({{ '/feral/pve/' | relative_url }}).

## My LIVE controls are OFF again

The session controls reset on every reload or relog. Set them again using the routine in [First Launch]({{ '/getting-started/first-launch/' | relative_url }}).

## Cyclone keeps getting interrupted

You moved during the cast. Stand still as soon as HOLD STILL appears. See the four-stage Cyclone on the [KORHTRAP]({{ '/hardkorh/korhtrap/' | relative_url }}) page.

## Diagnostics

- **KORHDIAG** writes a diagnostic log that records meaningful changes, such as a new decision, a cast result or a state change, rather than every frame. The first record of each session lists the plugin version, game version and your settings. With Verbose PvP Events ON, it also records spell-cast events.
- **Diagnostics Panel**: a denser HUD panel with the technical details behind each HUD row. Turn it on when support asks for a screenshot.
- **Status on the settings page**: every section shows its live status rows while the plugin is enabled. SYSTEM STATUS gives the short summary; SUPPORT DIAGNOSTICS holds collapsed sections for keybinds, the HARDKORHKIT composition (every subsystem's load status), targeting, control, defensives, burst, the executor and raw telemetry.
- The ADVANCED card, the Runtime Probe Key and the SUPPORT DIAGNOSTICS sections are for support. Change them only when support asks you to.

## Collecting logs

1. Keep **Diagnostic File Logging** ON (LOGGING & SUPPORT card). The log is written only while the plugin is enabled.
2. Reproduce the problem.
3. Before you reload, copy the log file from your Project Sylvanas folder: `scripts_log/hardkorh/feral_pvp.log`. The file holds the latest session only, so a reload starts it over.

On Balance, keep **Balance Diagnostic Logging** ON and copy `scripts_log/hardkorh/balance_pvp.log` instead.

## Resetting a single option

Right-click the option to reset it, or set it back to its default: Enable Plugin OFF; Combat HUD ON; Diagnostics Panel OFF; HUD 1 / 28 / 100; Cyclone cue and sound ON; Interrupt At Cast 70%; Logging ON; Verbose OFF; Decision Engine ON; Dry Run OFF; keybinds unbound. See [Settings]({{ '/hardkorh/settings/' | relative_url }}).

## Reporting a reproducible problem

Post it in **🐛・bug-fixes** on [Discord](https://discord.gg/sv2WNwk2WZ) with:

- what you expected and what happened, with the time;
- the HUD rows at that moment (a screenshot is ideal) and the session controls you had on;
- the log file from the same session;
- your specialization, and on Feral the build line from the top of the HARDKORH page, for example **HARDKORH PVP AIO v1.0.0 - Feral M6.6**.
