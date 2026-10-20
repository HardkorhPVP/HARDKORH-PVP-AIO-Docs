---
title: "The HARDKORH Platform"
permalink: /hardkorh/platform/
excerpt: "One PvP intelligence platform shared by every HARDKORH class pack: what each KORH subsystem does and how a decision is made."
toc: true
toc_label: "On this page"
---

HARDKORH is a PvP intelligence platform, not a rotation. One shared foundation observes the fight, decides what matters most right now, and acts through a single, careful execution layer. Each class pack adds the knowledge of its class and specializations on top of that foundation, so every specialization shares the same targeting, control, defensive, interrupt and display intelligence.

<div class="hk-pack">
  <span class="hk-pack__title">HARDKORH DRUID</span>
  <div class="hk-pack__specs">
    <a class="hk-spec hk-spec--done" href="{{ '/feral/required-talents/' | relative_url }}"><span class="hk-spec__name">FERAL</span><span class="hk-spec__state">DONE</span></a>
    <a class="hk-spec hk-spec--done" href="{{ '/balance/' | relative_url }}"><span class="hk-spec__name">BALANCE</span><span class="hk-spec__state">DONE</span></a>
    <span class="hk-spec hk-spec--planned"><span class="hk-spec__name">RESTORATION</span><span class="hk-spec__state">PLANNED (NEXT)</span></span>
  </div>
  <span class="hk-pack__note">Every class and specialization on the way: <a href="{{ '/roadmap/' | relative_url }}">Roadmap</a></span>
</div>

## How a decision is made

<ol class="hk-flow">
  <li><span>SEE</span></li>
  <li><span>THINK</span></li>
  <li><span>CHOOSE</span></li>
  <li><span>ARBITRATE</span></li>
  <li><span>EXECUTE</span></li>
  <li><span>SHOW</span></li>
  <li><span>RECORD</span></li>
</ol>

1. **See.** KORHSIGHT reads the fight: enemy and friendly players, their roles, who is in melee range of you, who is casting at whom, who is immune, crowd-controlled or behind a major defensive.
2. **Think.** KORHTHINK turns those facts into what the moment calls for: building pressure, setting up control, bursting, defending, stabilizing or recovering.
3. **Choose.** Each specialist proposes its best action for that objective: KORHTRAP for crowd control, KORHSHIELD for survival, KORHKICK for interrupts, KORHUSE for items, and the class pack's own rotation for damage.
4. **Arbitrate.** Competing proposals are ranked. Survival comes first; a damage spell never takes the place of a needed defensive, and a low-value control never spends diminishing returns a coming kill window needs.
5. **Execute.** KORHGO casts the winning action, but only after its own checks pass.
6. **Show.** KORHVISION puts the objective, the action and the reason on your HUD.
7. **Record.** KORHDIAG writes what changed to a diagnostic log for support.

## The KORH subsystems

| Subsystem | Role | What it does for you |
| --- | --- | --- |
| **HARDKORHKIT** | Shared foundation | Assembles every subsystem, identifies what loaded and reports anything that did not. A missing part fails safe instead of acting half-informed. |
| **KORHGO** | Execution | The only part of HARDKORH that casts. It executes decisions; it never invents strategy. Every request must be an ability your specialization allows, learned, usable and castable on its target, and the game must confirm it. A refused or unconfirmed request is retried with care or dropped, never spammed. |
| **KORHSIGHT** | Observation | PvP unit and target awareness: who is a healer, who your damage is for, who is in melee range or targeting you, and each player's immunities and crowd-control state. |
| **KORHTHINK** | Strategy | Strategic PvP intelligence that coordinates offense, defense, control, burst, recovery and kill opportunities, so the other subsystems pull in the same direction. |
| **KORHTRAP** | Crowd control | Chooses who to control, when and with what: diminishing returns, immunities, crowd control already on the target, and setups such as controlling the healer before a burst. |
| **KORHSHIELD** | Defense | Reads your survival situation as a whole, not a single health number, and escalates defensives, heals and peels only as far as the situation needs. |
| **KORHKICK** | Interrupts | Decides which enemy cast is worth an interrupt or silence, and when in the cast, weighing who it targets and what is happening in the fight. |
| **KORHUSE** | Item use | Uses the Healthstone in your bags when the situation calls for it, not on a fixed reflex. |
| **KORHVISION** | Display | The combat HUD, on-screen cues and confirmed-outcome notifications. Display only: combat is identical with it hidden. |
| **KORHDIAG** | Diagnostics | Runtime telemetry and a change-based diagnostic log, so support can see what HARDKORH saw and why it acted. |

## How each specialization uses the platform

The subsystems are shared; how deeply each specialization uses them depends on the class. Behavior always follows the page of your specialization.

| | Feral | Balance |
| --- | --- | --- |
| **Master switch** | Enable Plugin | Balance Execution |
| **KORHSIGHT** | A sticky KILL target with Option C Live Targeting | Your current hostile target is the KILL; CONTROL and INTERRUPT targets are chosen separately |
| **KORHTHINK** | PvP facts and pressure context behind every Feral decision | One strategic objective at a time, with a policy for every subsystem ([Balance KORHTHINK]({{ '/balance/korhthink/' | relative_url }})) |
| **KORHTRAP** | Incapacitating Roar and a four-stage Cyclone on the enemy healer | Offensive and defensive Cyclone, Root + Beam, peels and Typhoon ([Balance control]({{ '/balance/control-and-korhkick/' | relative_url }})) |
| **KORHSHIELD** | Barkskin, Survival Instincts, Healthstone, Regrowth and an owned defensive Bear | Barkskin, peels, Regrowth, Healthstone, an owned defensive Bear with Frenzied Regeneration and Heart of the Wild ([Balance KORHSHIELD]({{ '/balance/korhshield/' | relative_url }})) |
| **KORHKICK** | Skull Bash at the cast progress you choose | Solar Beam, aware of who the cast targets and whether it is crowd control |
| **Burst** | [Arena Burst]({{ '/hardkorh/arena-burst/' | relative_url }}) kill windows | The Eclipse cycle and charge-aware Incarnation ([Eclipse & Burst]({{ '/balance/eclipse-and-burst/' | relative_url }})) |

## How HARDKORH behaves

- **Observed facts, not guesses.** Every decision rests on what the game reports. When something cannot be read, HARDKORH treats it as unknown and does not act on it: it fails closed.
- **Read live, never assumed.** Learned abilities, charges, cooldowns, cast times, costs and resource limits are read from your client while you play.
- **Your hands stay in charge.** HARDKORH never moves your character, navigates, turns you to face a target, or changes your WoW target or focus.
- **Success means seen.** A success message, such as a confirmed Cyclone, appears only after HARDKORH has seen the effect on the enemy, never just because a spell was sent.
- **One master switch per specialization.** Turning it off stops every decision and cast at once.
- **Built for PvP.** The intelligence is designed for Arena, Solo Shuffle, Battlegrounds and world PvP. Combat abilities still work outside PvP, but there is no dungeon or raid logic.

## Class packs

HARDKORH is organized as one shared platform plus class packs. A class pack covers one class and contains every HARDKORH specialization of that class: **HARDKORH Druid** contains Feral and Balance today, with Restoration planned next. Only damage and healing specializations are built; tank specializations are not part of HARDKORH.

**HARDKORH PVP AIO** brings together every available class pack. Pricing and availability of individual class packs will be announced when they are finalized.

See the [Roadmap]({{ '/roadmap/' | relative_url }}) for every class and specialization on the way.
