---
title: "Keybinds"
permalink: /getting-started/keybinds/
excerpt: "Four player keybinds, each toggling exactly one setting."
---

HARDKORH Feral has four independent player keybinds. Each one toggles exactly one setting, the same setting as its switch. Pressing the key and clicking the switch are interchangeable. All four work with the menu closed, and holding a key down does not repeat the toggle.

HARDKORH Balance has one keybind, the **Balance Execution Key**, which turns Balance Execution on or off. See [Balance Settings]({{ '/balance/settings/' | relative_url }}).

| Keybind | Card | Toggles | Default |
| --- | --- | --- | --- |
| **Enable Plugin Key** | GENERAL OPTIONS | Enable Plugin, the master switch (LIVE or DISABLED) | Unbound |
| **Combat HUD Key** | KORHVISION | Combat HUD shown or hidden | Unbound |
| **Diagnostics Panel Key** | KORHVISION | Diagnostics Panel on or off | Unbound |
| **Arena Burst Key** | BURST | Arena Burst ON or OFF (this session; OFF again after every reload) | Unbound |

## Assigning a key

You choose your own keys; none is required. Click the keybind field on the HARDKORH page, then press the key you want. The key is saved between sessions. Pick keys you can reach in combat and that are not used by anything else.

## Active purple, inactive gray

The Project Sylvanas menu highlights a keybind **purple** when it is active and **gray** when it is inactive. HARDKORH keeps that highlight in step with the setting the key controls:

- purple = the setting is ON (plugin enabled, HUD shown, Diagnostics Panel on, Arena Burst on);
- gray = the setting is OFF.

The highlight follows key presses, checkbox clicks, reloads and resets. If it ever disagrees with the setting, the setting is still correct. See [Troubleshooting]({{ '/support/troubleshooting/' | relative_url }}).

{% include hk-figure.html src="/assets/images/screenshots/03-keybind-states.png" alt="KORHVISION keybinds: the Combat HUD Key highlighted purple and the Diagnostics Panel Key gray" w="531" h="106" class="hk-figure--small" caption="Purple means the setting is ON (Combat HUD); gray means OFF (Diagnostics Panel)." %}

## What the keys never do

- The Enable key never changes the HUD or the Diagnostics Panel.
- The HUD key never changes Enable Plugin or the Diagnostics setting.
- The Diagnostics key never shows or hides the HUD itself. The panel draws only inside a visible HUD.
- The Arena Burst key never changes anything except Arena Burst.

<div class="notice--info" markdown="1">
**Instant manual control.** Your Enable Plugin key is the fastest way to take over: one press stops everything, another press resumes LIVE.
</div>
