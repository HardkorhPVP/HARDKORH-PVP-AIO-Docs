---
title: "FAQ"
permalink: /support/faq/
excerpt: "Short answers to the questions players ask most."
---

### Which specializations are supported?
Feral Druid and Balance Druid are done. Restoration Druid is planned next, and more classes are on the [Roadmap]({{ '/roadmap/' | relative_url }}). Tank specializations are not planned.

### Does HARDKORH move or turn my character?
No. Movement, facing and positioning are always yours.

### Does it change my target?
No. It never changes your WoW target or focus. On Feral, with Option C LIVE it chooses whom its damage goes to, and your own target switch always wins. On Balance, your current target receives your damage, and crowd control and interrupts are cast directly at the units HARDKORH chooses for them.

### Do I need the required talent build?
On Feral, yes, for the documented behavior. HARDKORH was built and tested on exactly one Feral talent setup, and it only uses abilities you have learned. Another build still loads the plugin, but no other build has been validated. Import the code on [Required Talents]({{ '/feral/required-talents/' | relative_url }}). On Balance, HARDKORH uses the abilities you have learned; see [abilities HARDKORH Balance can use]({{ '/balance/#abilities-hardkorh-balance-can-use' | relative_url }}).

### What is KILL vs CONTROL?
KILL is your damage target. CONTROL is the crowd-control target: on Feral with CC Healer ON it is the enemy healer. They can be different players at the same time, and your damage does not move to the healer because it is the CONTROL target. See [KORHSIGHT]({{ '/hardkorh/korhsight/' | relative_url }}). Balance adds a third role, INTERRUPT, for Solar Beam; see [Balance control]({{ '/balance/control-and-korhkick/#three-targets-kept-separate' | relative_url }}).

### Why did Cyclone ask me to stop?
Cyclone is a hard cast. HOLD STILL means a Cyclone is ready and waiting for you; STOP MOVING means the cast is starting. Moving cancels the cast, so plant your feet until the cue clears. See [KORHTRAP]({{ '/hardkorh/korhtrap/' | relative_url }}) for Feral and [Balance control]({{ '/balance/control-and-korhkick/#your-part-stand-still-for-cyclone' | relative_url }}) for Balance.

### Why didn't it Cyclone the healer?
On Feral, check that CC Healer and Cyclone Live are ON, that you are standing still with line of sight within range, and that the healer is not immune or on long diminishing returns. On Balance, read the KORHTHINK and CONTROL PLAN rows: survival may come first, or HARDKORH may be saving diminishing returns for your next burst.

### Why did it stop attacking?
On Feral, read the HOLD row. Common reasons: the KILL is immune, in Cyclone or breakable CC; you are stunned; a Cyclone cast is running; you are not in Cat Form. On Balance, read the KORHTHINK and REASON rows: for example, HARDKORH does not damage a kill target that is in Cyclone or immune.

### Why did HARDKORH enter Bear Form?
Defensives always outrank damage. On Feral, under PvP pressure in combat, at around 40% health, KORHSHIELD can take you into a defensive Bear Form that it owns (BEAR reads OWNED), runs the Bear tools, and returns you to Cat once you are back above about 70% health. Do not cancel it while BEAR reads OWNED. See [KORHSHIELD]({{ '/hardkorh/korhshield/' | relative_url }}). On Balance, an emergency can call for a defensive Bear too, and HARDKORH returns you to Moonkin when it is safe; Incapacitating Roar also shifts you into Bear briefly. See [Balance KORHSHIELD]({{ '/balance/korhshield/' | relative_url }}).

### Is Arena Burst automatic?
On Feral, only after you turn it on. Arena Burst is a session-only switch (or its key) that returns to OFF on every reload. With it ON and CC Healer ON, HARDKORH spends Incarnation or Berserk in an authorized kill window while the enemy healer is crowd-controlled. Against a team without a healer, the Arena logic does not burst. See [Arena Burst]({{ '/hardkorh/arena-burst/' | relative_url }}).

### Does Balance use Incarnation automatically?
Yes, with Balance Execution ON and an enemy player as your target. HARDKORH reads Incarnation's charges live, prepares the window, and can wait briefly for healer control, but never wastes a charge waiting. See [Eclipse & Burst]({{ '/balance/eclipse-and-burst/#incarnation-charge-aware-burst' | relative_url }}).

### What do KILL WINDOW and STABILIZING mean?
They are the two strategic cues of HARDKORH Balance. KILL WINDOW: your burst is running and the enemy healer is controlled or absent, or your kill target is low. STABILIZING: survival comes first right now. See [KORHTHINK]({{ '/balance/korhthink/' | relative_url }}).

### Does HARDKORH Balance cast Starfall or Ursol's Vortex?
No. Starfall and Ursol's Vortex stay manual, and so does Force of Nature when the game reports it as ground-targeted. See [Scope & Limits]({{ '/balance/scope-and-limits/' | relative_url }}).

### Why are my LIVE controls off after a reload?
On Feral, they are session-only by design, so every session starts safe. Enable Plugin and all other settings are saved. Balance has no session-only controls: Balance Execution and the other Balance settings are saved.

### Does Enable Plugin need an extra arm click?
No. Enable Plugin ON is LIVE. On Balance, Balance Execution ON is LIVE.

### Does HARDKORH work in PvE?
The rotation and defensives work on your target, but there is no dungeon- or raid-specific logic. HARDKORH is built for PvP. See [PvE]({{ '/feral/pve/' | relative_url }}) for Feral and [Scope & Limits]({{ '/balance/scope-and-limits/' | relative_url }}) for Balance.

### Which Project Sylvanas version should I use?
The latest available version. Update Project Sylvanas before using HARDKORH; no compatibility claim is made for older builds.

### Where do I get support?
On [Discord](https://discord.gg/sv2WNwk2WZ): questions in **🆘・support**, reproducible bugs in **🐛・bug-fixes**. See [Troubleshooting]({{ '/support/troubleshooting/' | relative_url }}) for what to include.

### Is it safe to use?
HARDKORH makes no safety or detection claims. It is third-party automation software; using it may violate the World of Warcraft Terms of Use, and you use it at your own risk.
