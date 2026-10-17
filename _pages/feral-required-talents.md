---
title: "Required Talents"
permalink: /feral/required-talents/
excerpt: "The required HARDKORH Feral talent build. World of Warcraft 12.1.5, Midnight Season 2."
---

<div class="notice--primary" markdown="1">
**Required HARDKORH Feral talent build**

HARDKORH was built and tested on exactly one Feral talent setup, the build below, and its combat logic assumes that build. For the documented and validated HARDKORH behavior, use the supplied build, and import it before your first session.
</div>

## Talent import code

World of Warcraft 12.1.5 · Midnight Season 2

<pre class="hk-talent-code"><code>CcGADBD3hSPCL9Y9gz68WcKvMAAAAAAwYMzCjZmZG2WYZmlZmZMzMAAAAsEMbGYmZqZMbmZmZWGz8AGAAAAAAgBAAAQGz2MmZ2mZpZbmlNYmZAWYwAAYmBzsgB</code></pre>

Click the code once to select all of it, then copy. It is a single unbroken line; paste it exactly as shown, without spaces or line breaks.

## How to import

1. Copy the import code above.
2. In World of Warcraft, open the talent window and use the import option to paste the code.
3. Apply the loadout, and reload so HARDKORH re-reads your learned abilities.

{% include hk-figure.html src="/assets/images/screenshots/10-talent-tree.png" alt="The World of Warcraft talent window with the required HARDKORH Feral build: Druid class tree, Wildstalker hero tree, Feral specialization tree and three PvP talents" w="1593" h="839" caption="Required HARDKORH Feral talent build - WoW 12.1.5 / Midnight Season 2." %}

## Why this build matters

HARDKORH looks at which abilities you have actually learned and only ever uses those. Another build will still load the plugin, but the behavior described in this documentation is the behavior of this build:

- If you drop a talent HARDKORH expects, the logic tied to that ability has nothing to cast and stays idle.
- If you swap talents that change how an ability works, HARDKORH can behave differently from what is described here and from what was validated.

No other build has been validated, so no compatibility claims are made for alternative builds.

## Abilities HARDKORH can use

HARDKORH checks at runtime which of these you have learned and uses only those:

- **Cat:** Rake, Rip, Ferocious Bite, Shred, Moonfire (with Lunar Inspiration), Tiger's Fury, Feral Frenzy, Berserk / Incarnation.
- **Bear:** Mangle, Thrash, Swipe, Strength of the Wild, Typhoon, Heart of the Wild.
- **Cat or Bear:** Skull Bash, Wild Charge, Incapacitating Roar.
- **Other:** Cyclone, Barkskin, Survival Instincts, Frenzied Regeneration, Regrowth, Mark of the Wild, Bear Form, Cat Form.
- **Procs it reacts to:** Clearcasting (Omen of Clarity) and Predatory Swiftness.
