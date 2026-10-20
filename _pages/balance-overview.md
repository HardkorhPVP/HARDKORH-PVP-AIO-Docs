---
title: "Balance Druid"
permalink: /balance/
excerpt: "HARDKORH Balance: a PvP intelligence system for Balance Druid, not a damage priority list."
toc: true
toc_label: "On this page"
---

<span class="hk-pill hk-pill--live">DONE</span> &nbsp;Part of the **HARDKORH Druid** class pack, alongside [Feral]({{ '/feral/required-talents/' | relative_url }}).

HARDKORH Balance is a PvP intelligence system, not a damage priority list. It builds pressure with Astral Power, Eclipse and damage over time, chooses the moment to spend Incarnation, controls the enemy healer and the enemy who is bursting you, silences the casts that matter, and keeps you alive with defense that escalates only as far as the situation needs. **KORHTHINK** ties it together: one strategic objective at a time, with every part of HARDKORH working toward it.

Movement, positioning, facing and target choice stay in your hands.

## What HARDKORH Balance does

<div class="hk-cards">
  <a class="hk-card" href="{{ '/balance/eclipse-and-burst/' | relative_url }}"><span class="hk-card__name">SMART PRESSURE</span><span class="hk-card__line">Astral Power management, deliberate Eclipse use, Moonfire and Sunfire upkeep and steady pressure on your target.</span></a>
  <a class="hk-card" href="{{ '/balance/eclipse-and-burst/#incarnation-charge-aware-burst' | relative_url }}"><span class="hk-card__name">INTELLIGENT BURST</span><span class="hk-card__line">Charge-aware Incarnation, prepared resources, healer control first, a viable kill target and a real kill window.</span></a>
  <a class="hk-card" href="{{ '/balance/korhthink/' | relative_url }}"><span class="hk-card__name">KORHTHINK</span><span class="hk-card__line">One objective at a time: prepare, pressure, set up, burst, defend, stabilize, recover. Objectives first, spells second.</span></a>
  <a class="hk-card" href="{{ '/balance/control-and-korhkick/' | relative_url }}"><span class="hk-card__name">CONTROL</span><span class="hk-card__line">Cyclone with live Midnight diminishing returns, Root + Beam, Mighty Bash or Incapacitating Roar, roots and Typhoon.</span></a>
  <a class="hk-card" href="{{ '/balance/control-and-korhkick/#korhkick-solar-beam' | relative_url }}"><span class="hk-card__name">KORHKICK</span><span class="hk-card__line">Solar Beam on the casts that matter, with its own interrupt target and recognition of proven crowd-control casts.</span></a>
  <a class="hk-card" href="{{ '/balance/korhshield/' | relative_url }}"><span class="hk-card__name">KORHSHIELD</span><span class="hk-card__line">Barkskin, peels, Regrowth and a defensive Bear with Frenzied Regeneration, then back to Moonkin and back to pressure.</span></a>
  <a class="hk-card" href="{{ '/balance/korhvision/' | relative_url }}"><span class="hk-card__name">KORHVISION</span><span class="hk-card__line">The KORHTHINK objective on your HUD, KILL WINDOW and STABILIZING cues, and notifications for control that really landed.</span></a>
</div>

## How HARDKORH thinks

HARDKORH does not fire a spell because a number crossed a line. It reads the whole situation, decides what the moment is for, and only then picks the action. Two examples:

**Under pressure.** It weighs your health and how fast it is falling, the enemy cooldowns aimed at you, how many enemies are on you, whether your healer is free, which defensives you have left, your current form, and what offense it would give up. Then it escalates only as far as needed:

<ol class="hk-flow hk-flow--defense">
  <li><span>PRESSURE</span></li>
  <li><span>BARKSKIN</span></li>
  <li><span>PEEL / INSTANT HEAL</span></li>
  <li><span>EMERGENCY BEAR</span></li>
  <li><span>FRENZIED REGENERATION</span></li>
  <li><span>STABILIZE</span></li>
  <li><span>RECOVER</span></li>
  <li><span>MOONKIN</span></li>
  <li class="hk-flow__goal"><span>RETURN TO PRESSURE</span></li>
</ol>

**Going for a kill.** It weighs your DoTs, Astral Power, Eclipse, Incarnation charges and the risk of wasting one, whether the enemy healer can be controlled, whether your kill target is immune or behind a defensive, and whether you are safe enough to commit:

<ol class="hk-flow hk-flow--burst">
  <li><span>PREPARE</span></li>
  <li><span>CONTROL SETUP</span></li>
  <li><span>HEALER CONTROL</span></li>
  <li><span>INCARNATION / ECLIPSE</span></li>
  <li class="hk-flow__goal"><span>KILL WINDOW</span></li>
</ol>

More: [KORHTHINK]({{ '/balance/korhthink/' | relative_url }}), [KORHSHIELD]({{ '/balance/korhshield/' | relative_url }}) and [Eclipse & Burst]({{ '/balance/eclipse-and-burst/' | relative_url }}).

## Who does what

| HARDKORH handles | You handle |
| --- | --- |
| Moonkin Form, Moonfire, Sunfire, Wrath, Starfire, Starsurge, Eclipse and Incarnation | **All movement and positioning:** line of sight, pillars, range |
| Cyclone, roots, Solar Beam, Incapacitating Roar or Mighty Bash, Typhoon and Soothe, on the unit it chooses | **Facing:** Typhoon is used only when you already face the target |
| Barkskin, Regrowth, Healthstone, a defensive Bear Form with Frenzied Regeneration and Heart of the Wild | **Target choice:** your current target is the one your damage goes to |
| Mark of the Wild, and Remove Corruption on yourself | **Standing still** when the Cyclone cue asks |
| The return to Moonkin after its own Bear Form | Abilities HARDKORH does not cast, such as Starfall, Ursol's Vortex and trinkets ([Scope & Limits]({{ '/balance/scope-and-limits/' | relative_url }})) |

## Getting started on Balance

1. **Switch to Balance.** HARDKORH loads for the specialization you are in; changing specialization reloads it.
2. **Open the Balance settings.** In the Project Sylvanas menu, open **HARDKORH PVP AIO - BALANCE**. Balance keeps its own settings: the Feral page does not appear while you are Balance, and the Balance page does not appear while you are Feral.
3. **Turn on Balance Execution** with its switch or the Balance Execution Key. The HUD badge reads <span class="hk-pill hk-pill--live">LIVE</span>.
4. **Target the enemy you want to kill.** Your current hostile target receives your damage. HARDKORH picks its crowd-control and interrupt targets separately, and it never changes your target.
5. **Play.** Move, position and choose your fights. The first HUD row, KORHTHINK, tells you what HARDKORH is trying to do.

<div class="notice--info" markdown="1">
**One switch for everything**

Balance has a single master switch. Balance Execution ON runs the rotation, burst, crowd control, interrupts and defensives together; there are no extra per-session LIVE switches to remember. It is OFF on a new install. See [Balance Settings]({{ '/balance/settings/' | relative_url }}).
</div>

## Abilities HARDKORH Balance can use

HARDKORH checks at runtime which abilities you have learned, and uses only those. An ability you have not learned simply stays idle.

- **Pressure:** Moonfire, Sunfire, Wrath, Starfire, Starsurge, Solar and Lunar Eclipse, Incarnation: Chosen of Elune.
- **Control:** Cyclone, Entangling Roots, Mass Entanglement, Solar Beam, Incapacitating Roar or Mighty Bash (whichever your talents give you), Typhoon, Soothe.
- **Survival:** Barkskin, Bear Form, Frenzied Regeneration, Regrowth, Heart of the Wild, Healthstone.
- **Utility:** Moonkin Form, Mark of the Wild, Remove Corruption on yourself.
- **Opportunities it reacts to:** when the game reports a Starsurge that costs nothing, or a spell that casts instantly, HARDKORH uses that opportunity.

Force of Nature is used only if the game reports it as a targeted spell. When the game reports it as ground-targeted, the HUD shows it as not automated and it stays yours to cast. See [Scope & Limits]({{ '/balance/scope-and-limits/' | relative_url }}).

## Recommended build and gear

HardkorhPVP recommends a Keeper of the Grove PvP talent build and a Versatility / Haste PvP gearing plan for HARDKORH Balance. Neither is required for HARDKORH to work. See [Talents & Build]({{ '/balance/talents/' | relative_url }}) and [PvP Gear & Stats]({{ '/balance/gear-and-stats/' | relative_url }}).

<div class="notice--warning" markdown="1">
No rating, win rate or outcome is guaranteed. Results depend on your build, gear, connection, positioning and decisions.
</div>
