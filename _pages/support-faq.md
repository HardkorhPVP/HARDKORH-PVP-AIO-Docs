---
title: "FAQ"
permalink: /support/faq/
excerpt: "Short answers to the questions players ask most."
---

### Does HARDKORH move or turn my character?
No. Movement, facing and positioning are always yours.

### Does it change my target?
No. It never changes your WoW target or focus. With Option C LIVE it chooses whom its damage goes to, and your own target switch always wins.

### Do I need the required talent build?
Yes, for the documented behavior. HARDKORH was built and tested on exactly one Feral talent setup, and it only uses abilities you have learned. Another build still loads the plugin, but no other build has been validated. Import the code on [Required Talents]({{ '/feral/required-talents/' | relative_url }}).

### What is KILL vs CONTROL?
KILL is your damage target. CONTROL is the crowd-control target: with CC Healer ON it is the enemy healer. They can be different players at the same time, and your damage does not move to the healer because it is the CONTROL target. See [KORHSIGHT]({{ '/hardkorh/korhsight/' | relative_url }}).

### Why did Cyclone ask me to stop?
Cyclone is a hard cast on the enemy healer. HOLD STILL means a Cyclone window is opening; STOP MOVING means the cast is starting. Moving cancels the cast, so plant your feet until the cue clears. See [KORHTRAP]({{ '/hardkorh/korhtrap/' | relative_url }}).

### Why didn't it Cyclone the healer?
Check that CC Healer and Cyclone Live are ON, that you are standing still with line of sight within range, and that the healer is not immune or on long diminishing returns.

### Why did it stop attacking?
Read the HOLD row. Common reasons: the KILL is immune, in Cyclone or breakable CC; you are stunned; a Cyclone cast is running; you are not in Cat Form.

### Why did HARDKORH enter Bear Form?
Defensives always outrank damage. Under PvP pressure in combat, at around 40% health, KORHSHIELD can take you into a defensive Bear Form that it owns (BEAR reads OWNED), runs the Bear tools, and returns you to Cat once you are back above about 70% health. Do not cancel it while BEAR reads OWNED. See [KORHSHIELD]({{ '/hardkorh/korhshield/' | relative_url }}).

### Is Arena Burst automatic?
Only after you turn it on. Arena Burst is a session-only switch (or its key) that returns to OFF on every reload. With it ON and CC Healer ON, HARDKORH spends Incarnation or Berserk in an authorized kill window while the enemy healer is crowd-controlled. Against a team without a healer, the Arena logic does not burst. See [Arena Burst]({{ '/hardkorh/arena-burst/' | relative_url }}).

### Why are my LIVE controls off after a reload?
They are session-only by design, so every session starts safe. Enable Plugin and all other settings are saved.

### Does Enable Plugin need an extra arm click?
No. Enable Plugin ON is LIVE.

### Does HARDKORH work in PvE?
The Cat rotation and defensives work on your target, but there is no dungeon- or raid-specific logic. HARDKORH is built for PvP. See [PvE]({{ '/feral/pve/' | relative_url }}).

### Does it support Balance or Restoration?
No. HARDKORH supports Feral only.

### Which Project Sylvanas version should I use?
The latest available version. Update Project Sylvanas before using HARDKORH; no compatibility claim is made for older builds.

### Where do I get support?
On [Discord](https://discord.gg/sv2WNwk2WZ): questions in **🆘・support**, reproducible bugs in **🐛・bug-fixes**. See [Troubleshooting]({{ '/support/troubleshooting/' | relative_url }}) for what to include.

### Is it safe to use?
HARDKORH makes no safety or detection claims. It is third-party automation software; using it may violate the World of Warcraft Terms of Use, and you use it at your own risk.
