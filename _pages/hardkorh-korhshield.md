---
title: "KORHSHIELD - Defensives"
permalink: /hardkorh/korhshield/
excerpt: "Layered defensives, the owned defensive Bear and the return to Cat."
toc: true
toc_label: "On this page"
---

**Feral Druid.** For Balance defenses, see [Balance KORHSHIELD]({{ '/balance/korhshield/' | relative_url }}).

Defensives always outrank damage. KORHSHIELD is fully automatic and has no settings of its own; the only related switch is the session-only **Strength of the Wild Live** in the KORHSHIELD card.

## The defensive layers

In the current build the stages are approximately:

| Defensive | Used around | Notes |
| --- | --- | --- |
| **Barkskin** | 50% health | The first layer. |
| **Bear Form** | 40% health under PvP pressure in combat | A defensive Bear owned by HARDKORH; see below. |
| **Frenzied Regeneration** | 40% health in owned Bear | Self-heal in Bear. |
| **Survival Instincts** | 30% health | The emergency layer. |
| **Healthstone** | 30% health | When a Healthstone is in your bags; usable while moving. |
| **Regrowth** | Any health with a Predatory Swiftness proc | An instant self-heal. In Arena it is deferred during a burst window while you are healthy. |

Once a defensive is accepted, HARDKORH holds that stage briefly until the effect is seen, so it does not stack defensives back to back.

## Bear authority: OWNED and MANUAL

HARDKORH distinguishes a Bear Form it entered itself (**OWNED**) from a Bear Form you entered (**MANUAL (UNOWNED)**):

- In owned Bear, it runs a Bear rotation (Mangle, Thrash, Swipe) and the Bear toolkit: Frenzied Regeneration, Heart of the Wild, Typhoon and, if enabled, Strength of the Wild.
- It holds Bear until you are back above about 70% health, then returns to Cat.
- A Bear you entered yourself is adopted only under PvP pressure at low health.
- During active PvP engagement, HARDKORH otherwise returns you to Cat.

Inside an owned Bear the defensive ladder still applies: if your health keeps falling, Survival Instincts and the other emergency layers come before any Bear damage or utility.

{% include hk-figure.html src="/assets/images/screenshots/16-owned-bear-stabilize.png" alt="Arena combat in Bear Form: DEFENSIVE reads BEAR STABILIZE 49%, BEAR reads OWNED, ACTION HEART OF THE WILD (PENDING) and UTILITY shows Heart of the Wild, Typhoon and Strength of the Wild" w="1495" h="522" caption="Owned Bear stabilization: KORHSHIELD has taken charge of a defensive Bear (DEFENSIVE BEAR STABILIZE, BEAR OWNED) and runs the Bear tools shown on the UTILITY row." %}

{% include hk-figure.html src="/assets/images/screenshots/17-owned-bear-emergency.png" alt="Arena combat at 12% health in Bear Form: DEFENSIVE reads SURVIVAL INSTINCTS, BEAR reads OWNED and ACTION SWIPE (BEAR)" w="1794" h="496" caption="Emergency escalation inside owned Bear: at 12% health DEFENSIVE reads SURVIVAL INSTINCTS. Survival always comes before Bear damage and utility." %}

## The Bear toolkit and utility

| Ability | In an owned Bear |
| --- | --- |
| **Frenzied Regeneration** | Self-heal at around 40% health. |
| **Heart of the Wild** | Used when it is ready. The exact spell is identified from your client at login. |
| **Typhoon** | When the KILL target is in range and in front of you. HARDKORH never turns you to face it. |
| **Strength of the Wild** | With Strength of the Wild Live ON: with a KILL target in reach, unprotected, the spell ready and no survival action pending, it is cast ahead of Mangle. |

The HUD's **BEAR** row reads OWNED, REQUESTED, RECOVERY (TO CAT), MANUAL (UNOWNED) or NONE; the **UTILITY** row shows Heart of the Wild, Typhoon and Strength of the Wild while you are in owned Bear.

## Your responsibilities while defensive

- Break line of sight from the casters on you, and move toward your healer.
- Use the abilities HARDKORH does not cast, such as Dash, Stampeding Roar and trinkets, when the situation calls for them.
- Do not cancel Bear Form manually while BEAR reads OWNED; HARDKORH returns you to Cat when it is safe.
