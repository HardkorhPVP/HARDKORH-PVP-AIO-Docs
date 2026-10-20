---
title: "Requirements"
permalink: /getting-started/requirements/
excerpt: "What you need before your first HARDKORH session."
---

| Requirement | Detail |
| --- | --- |
| Product | **HARDKORH PVP AIO**, the latest version. |
| Class and specialization | A **Druid in Feral or Balance specialization**. HARDKORH loads only for those two; on any other class or specialization it stays inactive. More classes are on the [roadmap]({{ '/roadmap/' | relative_url }}). |
| Game | **World of Warcraft: Midnight**. This documentation covers World of Warcraft 12.1.5, Midnight Season 2. |
| Platform | The **latest available Project Sylvanas**. Keep Project Sylvanas updated before using HARDKORH; no compatibility claim is made for older or outdated Project Sylvanas builds. |
| Talents | Feral: the [required HARDKORH Feral talent build]({{ '/feral/required-talents/' | relative_url }}). Balance: the [recommended HARDKORH Balance build]({{ '/balance/talents/' | relative_url }}) (not required). HARDKORH checks at runtime which abilities you have learned and never uses an ability you do not have. |

## Safe by default

<div class="notice--info" markdown="1">
**Default disabled**

A new install, or a reset of the settings, starts with **Enable Plugin OFF**. While it is off, HARDKORH decides nothing and casts nothing. The Combat HUD stays visible and reads <span class="hk-pill hk-pill--disabled">DISABLED</span>, so you always know the state.

On Balance, the master switch **Balance Execution** starts OFF in the same way.
</div>

## The LIVE contract

<div class="notice--success" markdown="1">
**Enable Plugin = LIVE**

Turning **Enable Plugin** ON puts HARDKORH straight into LIVE operation. There is no second arm step. Turning it OFF stops all automation at once and clears any pending request.
</div>

On Feral, a few advanced features also have their own **session-only LIVE controls**: Option C Live Targeting, CC Healer, Incapacitating Roar Live, Cyclone Live, Arena Burst and Strength of the Wild Live. They start OFF after every reload by design. [First Launch]({{ '/getting-started/first-launch/' | relative_url }}) shows the per-session routine.

On Balance, **Balance Execution** is the one master switch, with no extra session-only controls. See [Balance Settings]({{ '/balance/settings/' | relative_url }}).

Next: [Installation]({{ '/getting-started/installation/' | relative_url }}).
