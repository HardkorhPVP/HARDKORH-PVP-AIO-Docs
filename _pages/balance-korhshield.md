---
title: "Balance KORHSHIELD"
permalink: /balance/korhshield/
excerpt: "Situation-aware defense for Balance: Barkskin, peels, heals, a defensive Bear and the way back to pressure."
toc: true
toc_label: "On this page"
---

<div class="notice--primary" markdown="1">
**Not "Barkskin at 50%"**

A fixed health line is the easiest defensive rule to write and the easiest to punish. It fires Barkskin into nothing when you are only chipped, and fires too late when a coordinated go is already killing you. KORHSHIELD reads the whole survival situation instead, and escalates only as far as that situation needs.
</div>

## What KORHSHIELD reads

- **Your health**, and **how fast it is falling** over the last couple of seconds.
- **Enemy burst:** an offensive cooldown aimed at you.
- **Who is on you:** how many enemies are in melee range or targeting you.
- **Your healer:** free, controlled, or not there.
- **What you have left:** which defensives and heals are ready.
- **Your form:** Moonkin, caster, a Bear HARDKORH entered, or a form you chose yourself.
- **What it would cost:** the offense a defensive global cooldown gives up, especially during your own burst.

From these it rates your situation as **NORMAL**, **PRESSURED**, **DANGER** or **EMERGENCY**. It escalates the moment the evidence appears, and steps down only after the pressure has stayed gone for a moment, so it does not flicker between levels.

## The escalation

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

Not every fight climbs every step. A burst that is already biting may only need an early Barkskin; a melee training you with your healer stunned may need a peel, a heal and a Bear. When the danger passes, HARDKORH brings you back to Moonkin and back to pressure.

## The tools

| Tool | How KORHSHIELD uses it |
| --- | --- |
| **Barkskin** | Proactively, when enemy burst on you is already landing, not on trivial pressure. Always in an emergency. Off the global cooldown, in any form, and even while you are stunned. |
| **Peels** | When an enemy is in melee range of you and you are in danger: Incapacitating Roar or Mighty Bash, Mass Entanglement, Typhoon when you face the enemy, Entangling Roots. Planned with the [control tools]({{ '/balance/control-and-korhkick/#peels' | relative_url }}). |
| **Regrowth (instant)** | When the game reports Regrowth as instant, it is a movement-safe heal used when you genuinely need healing. |
| **Regrowth (hard cast)** | Only with a real need, while you are standing still, with at most one enemy in melee on you, and never while enemy burst is on you or a melee is on you in danger. It is never spammed and never used at high health. |
| **Healthstone** | In danger or emergency at low health, in any form, when one is in your bags. |
| **Bear Form** | A defensive Bear that HARDKORH owns, entered when an emergency or serious danger calls for it: enemy burst on you, several enemies in melee, or your healer controlled. Never from Cat or Travel Form, and never cast again while you are already a Bear. |
| **Frenzied Regeneration** | In Bear Form when healing is needed and its heal is not already running, including in a Bear you entered yourself. |
| **Heart of the Wild** | Inside HARDKORH's own defensive Bear, as a major survival response, when it is ready. |
| **Remove Corruption** | On yourself, for a curse or poison the game identifies, when it is worth the global cooldown. |
| **Mark of the Wild** | Out of combat, when it is missing. |

While you are stunned, KORHSHIELD limits itself to the tools that can work through the stun, such as Barkskin.

## The defensive Bear

### HARDKORH's Bear, or yours

HARDKORH distinguishes a Bear Form it entered itself from a Bear Form you chose:

- **HARDKORH's own Bear** (from KORHSHIELD, or from its own Incapacitating Roar) is held while the reason for it lasts. Then HARDKORH returns you to Moonkin.
- **A Bear you entered yourself** is never cancelled and never taken over. Frenzied Regeneration can still heal you in it, but HARDKORH leaves the form to you.

The same respect applies to Cat Form and Travel Form: HARDKORH does not shift you out of a form you chose.

### Commitment without flip-flopping

Once an emergency calls for the Bear, that decision is held for a short, bounded time. A single heal tick that lifts your health for a moment does not cancel it while you are still under real pressure. The commitment ends as soon as the Bear is up, the pressure resolves, the Bear is unavailable, or the time runs out. HARDKORH also does not re-enter a Bear right after leaving its own, unless it is an emergency.

### Survival keeps its global cooldown

When the objective is **STABILIZE** and a survival action is waiting, because the global cooldown is running, an attempt was refused and is about to retry, or you are stunned, a new damage spell does not take that global cooldown. Emergency control can still act, the return to Moonkin is never held, and the reservation is short so the rotation never freezes.

## What defense costs offense

- No new Incarnation starts while KORHSHIELD reads DANGER or EMERGENCY. An Incarnation that is already running is never cancelled.
- During your own burst, only survival actions, and defensives that are off the global cooldown or truly needed, interrupt it.
- After the danger, a short **RECOVERY** puts a needed heal before the next Eclipse, so you do not open a window at low health.
- HARDKORH never cancels a cast in progress to defend; it chooses the next action instead.

## On the HUD

| Row | Reads |
| --- | --- |
| **DEFENSE** | NORMAL, PRESSURED, DANGER or EMERGENCY, with the reason. |
| **DEFENSIVE ACTION** | The survival action chosen right now, a hold or wait with its reason, or NONE. |
| **HEALER** | Your own healer: FREE, CONTROLLED, or NONE when you have none. |
| **BEAR** | OFF, HARDKORH's own Bear with its reason, or MANUAL for a Bear you entered. |

The KORHTHINK row shows DEFENSE, STABILIZE or RECOVERY while survival is the objective, and a red **STABILIZING** cue appears when the fight turns critical. See [KORHVISION - HUD & Cues]({{ '/balance/korhvision/' | relative_url }}).

## Your part

- Break line of sight from the casters on you, and move toward your healer. HARDKORH never moves you.
- Use the abilities HARDKORH does not cast, such as trinkets and movement abilities, when the situation calls for them.
- Leave HARDKORH's own Bear to HARDKORH: it returns you to Moonkin when it is safe.
