---
title: "Balance Talents & Build"
permalink: /balance/talents/
excerpt: "The recommended HARDKORH Balance PvP build: Keeper of the Grove. World of Warcraft 12.1.5, Midnight Season 2."
toc: true
toc_label: "On this page"
---

<div class="notice--primary" markdown="1">
**Recommended HARDKORH Balance PvP build: Keeper of the Grove**

This is the Balance PvP talent build HardkorhPVP recommends for HARDKORH. It is a recommendation, not a requirement: HARDKORH Balance runs on whatever talents you choose, and Balance Execution does not depend on this build.
</div>

## Talent import code

World of Warcraft 12.1.5 · Midnight Season 2 · Hero talents: **Keeper of the Grove**

<pre class="hk-talent-code"><code>CYGADBD3hSPCL9Y9gz68WcKvMAAAAAAAAAAAAAAAAAWoMLNjxMDwsZmZmZjxwMLjlZMjZYmlZMzMD2wAgxy2M22mZbWmpZmlZCAAAwmZmZmBbGGjBgZGAYA</code></pre>

Click the code once to select all of it, then copy. It is a single unbroken line; paste it exactly as shown, without spaces or line breaks.

## How to import

1. Copy the import code above.
2. In World of Warcraft, open the talent window and use the import option to paste the code.
3. Apply the loadout, and reload so HARDKORH re-reads your learned abilities.

{% include hk-figure.html src="/assets/images/screenshots/19-balance-talent-tree.png" alt="The World of Warcraft talent window with the recommended HARDKORH Balance build: Druid class tree, Keeper of the Grove hero tree, Balance specialization tree and the PvP talent row" w="1603" h="854" caption="Recommended HARDKORH Balance PvP build, Keeper of the Grove - WoW 12.1.5 / Midnight Season 2. The import code above is the exact configuration." %}

## Why this build

HARDKORH Balance is built around a specific toolkit: Eclipse and Astral Power pressure, charge-aware Incarnation, Cyclone and the other crowd-control tools, Solar Beam, and a defensive layer of Barkskin, a defensive Bear and heals, all coordinated by KORHTHINK. The recommended build is the configuration HardkorhPVP pairs with that toolkit, so the behavior described in this guide has the tools it expects.

| HARDKORH system | Where it is explained |
| --- | --- |
| Eclipse, Astral Power and Incarnation | [Eclipse & Burst]({{ '/balance/eclipse-and-burst/' | relative_url }}) |
| Strategic objectives and priorities | [KORHTHINK]({{ '/balance/korhthink/' | relative_url }}) |
| Cyclone, roots, peels and Solar Beam | [Control & KORHKICK]({{ '/balance/control-and-korhkick/' | relative_url }}) |
| Barkskin, the defensive Bear and heals | [KORHSHIELD]({{ '/balance/korhshield/' | relative_url }}) |

### Keeper of the Grove

The build uses the **Keeper of the Grove** hero talents. HARDKORH does not hard-code hero talents. It reacts to what the game reports while you play: when a talent makes a Starsurge free or a spell instant, HARDKORH sees the new cost or cast time and uses the opportunity. Abilities that the game reports as ground-targeted, such as Force of Nature when it is, stay yours to cast; see [Scope & Limits]({{ '/balance/scope-and-limits/' | relative_url }}).

## Talent-aware, not talent-locked

- HARDKORH discovers your abilities from your live spell book at login, by their exact names, including the abilities your talents add or replace.
- An ability you have not learned is never requested. The logic tied to it stays idle, and the rest of HARDKORH keeps working: it fails closed.
- Where your talents offer a choice, such as Incapacitating Roar or Mighty Bash, HARDKORH uses whichever one you have.
- Another build still runs HARDKORH Balance; this page simply documents the build HardkorhPVP recommends.

After any talent change, reload so HARDKORH re-reads your spell book.

Next: [PvP Gear & Stats]({{ '/balance/gear-and-stats/' | relative_url }}).
