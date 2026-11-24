#Homebrew #Rules 
A Supplement for Large-Scale Warfare in Fifth Edition

## INTRODUCTION

War, in most campaigns, happens offscreen. An empire falls, a siege is won, a
thousand soldiers die — and the player characters hear about it in a letter.
*Banners in the Field* exists to put the players inside that war without
turning every battle into a session-long grind of extra rules.

This supplement gives you **two ways to run a battle**, chosen based on the
role the player characters have in it:

> ##### THE TWO MODES OF WAR
> **Participant Mode.** The characters are inside someone else's battle —
> mercenaries, soldiers, infiltrators. They don't command the army; they
> fight their own fight within it, and their actions bend the battle's
> momentum without controlling it outright. Resolved with the **Victory
> Flower** (Chapter 3).
>
> **Commander Mode.** The characters *are* the generals. They build armies,
> deploy them on a map, issue orders, and personally drop into the fighting
> whenever it matters most. Resolved with the **Warfront** rules (Chapters
> 5–7).

Both modes run on the same underlying building block — the **Squad**
(Chapter 2) — and both modes feed into the same campaign-scale structure,
the **War Council** (Chapter 1), which tracks how an entire war unfolds
across many battles without requiring you to resolve every last skirmish in
full detail.

---

# CHAPTER 1: THE WAR COUNCIL

A war is bigger than any single battle. The War Council rules model an
entire campaign of conflict — a disputed border, a siege campaign, a
continent-spanning invasion — as a grid of contested fronts, so that the
player characters' victories and losses accumulate into something larger
than the sum of their fights.

## THE WAR MAP

At the start of a war, draw a grid — a 3×3 grid is the standard, representing
nine fronts of the conflict, though a longer campaign can use a 4×4 or 5×5,
or an irregular shape fitted to the actual geography of the region at war.

Each cell of the grid is a **Front**. Give each Front three properties:

- **Objective** — what holding this Front represents (a keep, a river
  crossing, a stretch of farmland, a capital city)
- **Weight** — Minor, Major, or Decisive (see below)
- **State** — Enemy-Held, Contested, or Yours, tracked throughout the war

> ##### FRONT WEIGHT
> | Weight | Typical Position | Scoring Value |
> |---|---|---|
> | Minor | Edge fronts | 1 |
> | Major | Fronts adjacent to the center or corners | 2 |
> | Decisive | The center, or a designated capital/objective | 3 |

## THE WAR TURN

The campaign advances in **War Turns** — one turn per week, month, or
season of in-fiction time, at your discretion. Each War Turn has three
phases:

**1. Assignment.** The players decide which Fronts they will personally
attend this turn (run in either Participant or Commander Mode — see
Chapters 3 and 5) and which Fronts are left to resolve automatically. A
party can split up, with different characters attending different Fronts
in the same turn.

**2. Resolution.** Every active Front resolves simultaneously:

- Fronts attended by characters in **Participant Mode** resolve with the
  **Victory Flower** (Chapter 3).
- Fronts attended by characters in **Commander Mode** resolve on the
  **Warfront** hex map (Chapters 5–7).
- Unattended Fronts resolve with the **Quick Resolution** check below.
- Fronts already locked as Yours or Enemy-Held from a previous turn don't
  need to be resolved again unless something is actively challenging them.

**3. Adjacency & Decisive Check.** Apply adjacency modifiers and check
whether any Front has hit its fight limit (see below).

## QUICK RESOLUTION

For a Front nobody is personally attending, don't run a full battle.
Compare each side's total army strength (sum the Requisition cost of all
squads committed there — see Chapter 4) and roll:

**2d6 + 1 per 50 points of Requisition advantage your side holds**
(minimum +0, this can go negative for the enemy's advantage instead)

| Total | Result |
|---|---|
| 6 or less | Contested (no change) |
| 7–11 | Favorable shift (move one step toward Yours) |
| 12+ | Decisive — Front becomes Yours outright |

Run the inverse for the enemy's roll if you want contested Fronts to
potentially swing against the players, or simply have both sides roll and
compare margins.

## ADJACENCY

Once a Front locks to **Yours** or **Enemy-Held**, it applies a standing
modifier to every Front sharing an edge with it, for as long as it remains
in that state:

| Locked State | Effect on Adjacent Fronts |
|---|---|
| Yours | +1 to that Front's army-strength comparisons |
| Enemy-Held | -1 to that Front's army-strength comparisons |
| Weakened (see below) | +0 or -0; no numeric effect, but note it narratively |

## THE DECISIVE CHECK

Every Front has a **Fight Limit** — the maximum number of War Turns it can
remain Contested before being forced to a result. Two turns is standard;
three for a Decisive-weight Front you want to matter more.

When a Front hits its limit while still Contested, force the result based
on its current lean (its Victory Flower position, or its last Quick
Resolution margin):

| Current Lean | Forced Result |
|---|---|
| Favoring you | **Pyrrhic Secure** — you hold it, but it becomes **Weakened**: apply only half the normal adjacency bonus to its neighbors |
| Even | **Stalemate** — becomes permanently neutral; contributes no score, but still occupies the grid |
| Favoring the enemy | **Pyrrhic Loss** — enemy holds it, Weakened, same halved penalty to neighbors |

This guarantees the war cannot stall out indefinitely — every Front resolves
within a known number of turns.

## ENDING THE WAR

The war ends once every Front has locked (aside from permanent Stalemates).
Tally **Weight-scored** results: sum the Weight value of every Front you
hold, versus every Front the enemy holds.

| Result | Outcome |
|---|---|
| Clear majority, mostly clean Secures | Decisive victory |
| Narrow majority, several Pyrrhic results | Costly victory — carry consequences into the next arc |
| Even split | Negotiated peace / ceasefire |
| Clear minority | Defeat — territory lost, campaign continues in a new shape |

---

# CHAPTER 2: SQUADS

Whether a battle runs in Participant or Commander Mode, the forces involved
are built from the same unit: the **Squad** — a single statblock
representing a formation of anywhere from a dozen to a few hundred
combatants, built and run exactly like a monster.

## SQUAD STATISTICS

Every squad has:

- **Quality Die** — rolled as part of its attack, representing training and
  cohesion: **Levy (d6)**, **Regular (d8)**, **Veteran (d10)**, **Elite (d12)**
- **Power** — a flat bonus added to attack rolls
- **Defense** — the target number other squads must meet or beat to deal
  damage
- **Strength Points (SP)** — this squad's pool of abstracted casualties,
  typically 4–8
- **Morale** — a DC used for the squad's own saving throws against breaking
- **Traits** — 0–2 keyword abilities drawn from the list below
- **Movement** — hexes it may move per round (Warfront only)
- **Requisition Cost** — its price when building an army (Chapter 4)

## THE CONDITION TRACK

A squad degrades instead of dying all at once.

| State | Trigger | Effect |
|---|---|---|
| **Full Strength** | Above 50% SP | No penalty |
| **Battered** | At or below 50% SP | -2 Power and Defense; make a Morale save |
| **Broken** | At or below 25% SP, or failed a Morale save | May only Disengage or Retreat; make a Morale save if damaged again |
| **Routed** | 0 SP, or a second failed Morale save | Removed from the battle |

> ##### SIDEBAR: MORALE SAVES
> Roll d20, add any applicable bonuses (a nearby Banner trait, a Rally
> order, a Stratagem), and compare to the squad's Morale DC. A squad that
> watches an **allied** squad in the same hex (or zone) Break takes a
> -2 penalty on its own next Morale save — panic spreads.

## SQUAD TRAITS

| Trait | Effect |
|---|---|
| **Phalanx** | While Full Strength or Battered, this squad gets a reaction: an opportunity attack against any enemy entering or leaving its hex/zone |
| **Charge** | The first time this squad hits a target in the battle, that target is knocked prone and takes +1 damage die |
| **Volley** | Instead of a single attack, targets every enemy in range with a Dex save; failure deals full damage, success deals half |
| **Skirmish** | Ignores difficult terrain; can move through occupied hexes; ignores enemy Phalanx reactions |
| **Siege** | Has a recharge 5–6 attack that deals heavy damage and ignores Defense bonuses granted by terrain |
| **Banner/Unbreakable** | Automatically succeeds its first Morale save of the battle; while Full Strength, allies sharing its hex/zone get +1 on their Morale saves |

## BUILDING A SQUAD

Use existing monster-building guidance to set AC (as Defense), HP (as SP ×
a multiplier of your choice, typically ×10–15 for flavor purposes only —
the SP number is what matters mechanically), and attack bonus/damage
scaled to the party's tier exactly as you would for any encounter. Then
assign a Quality Die, Power, and 0–2 Traits to taste.

> ##### EXAMPLE SQUADS
> | Squad | Quality | Power | Defense | SP | Morale | Traits | Req. Cost |
> |---|---|---|---|---|---|---|---|
> | Border Levy Spears | d6 | +2 | 12 | 6 | 11 | — | 12 |
> | Royal Lancers | d10 | +4 | 14 | 5 | 14 | Charge | 19 |
> | Longbow Company | d8 | +3 | 11 | 5 | 12 | Volley | 16 |
> | The Warlord's Elite Guard | d12 | +6 | 17 | 7 | 16 | Banner, Phalanx | 30 |

## SKIRMISH SCALE

Whenever a player character personally engages a squad — whether dropping
into a Participant battle or zooming in during Commander Mode — stop using
abstract resolution and run a **normal 5e combat encounter**. The squad
fights as its statblock; the PC fights as themselves, on a real grid, with
real initiative. Damage dealt carries over directly against the squad's SP
pool (roughly 10% of its effective fighting strength per SP, as a GM
guideline), and a clearly decisive personal victory can force an immediate
Morale save or Condition Track step, scaled by tier:

| Party Tier | Decisive Personal Victory Effect |
|---|---|
| 1–4 | Forces one Morale save |
| 5–10 | Forces one Morale save; may Batter the squad directly |
| 11–16 | Automatically Batters the squad |
| 17–20 | Automatically Breaks the squad, or ends the battle outright if a named enemy commander or Signature Unit (Chapter 4) is destroyed |

---

# CHAPTER 3: THE VICTORY FLOWER (PARTICIPANT MODE)

When the characters are inside someone else's battle — mercenaries,
conscripts, infiltrators — the battle's overall outcome is tracked with a
**Hex Flower**, a single token drifting across nineteen hexes that
represents the army's collective morale and momentum.

## THE FLOWER

> ##### HEX FLOWER LAYOUT
> - **Center hex:** Start
> - **Top hex (green):** Won — the army achieves total victory
> - **Bottom hex (red):** Lost — the army breaks
> - **Ring of six (blue):** Favorable momentum
> - **Ring of six (grey):** Even, grinding stalemate
> - **Ring of six (yellow):** Unfavorable momentum

Each ring hex has its own 2d6 **Navigation Hex** printed around it (per the
original Goblin's Henchman hex-flower design), indicating which direction
the token moves on a given roll.

## RESOLVING A ROUND

At the end of each round of the characters' personal combat:

**1. Determine Navigation Hex.** If the characters' side won the tactical
exchange this round, use the **Won (green) Navigation Hex**; if they lost
it, use the **Lost (red) Navigation Hex**.

**2. Roll 2d6 and apply modifiers:**

| Modifier | Value |
|---|---|
| Army power advantage/disadvantage | +1 / -1 |
| PCs achieved a strategic objective this round (held a position, killed an officer) | +1 |
| PCs lost a strategic objective this round | -1 |

**3. Move the token** the number of faces indicated, in the indicated
direction, wrapping around the flower unless an 'x' marks that face as
disallowed (in which case the token holds in place).

## MOMENTUM EFFECTS

The hex the token currently occupies applies a mechanical effect to the
characters' own combat rolls for the following round:

| Zone | Effect |
|---|---|
| Green | Battle ends — victory |
| Blue | +2 to the characters' attack rolls |
| Grey | No effect |
| Yellow | -2 to the characters' attack rolls |
| Red | Battle ends — defeat/retreat |

## TIER-SCALED HEROISM

A decisive personal action can nudge the token beyond the normal roll:

| Party Tier | Bonus Effect |
|---|---|
| 1–4 | +1 extra hex toward green/blue on a decisive success |
| 5–10 | As above, plus forces an immediate Morale save on one enemy squad |
| 11–16 | +2 extra hexes, and automatically Batters one enemy squad |
| 17–20 | Killing a named enemy commander can move the token straight to the green or red edge, ending the battle immediately |

## OPTIONAL ROUND LIMIT

If after a set number of rounds (6 is typical) the token hasn't reached
green or red, force a result exactly as the War Council's Decisive Check
does: blue resolves as a Pyrrhic win, yellow as a Pyrrhic loss, grey as a
stalemate.

---

# CHAPTER 4: ARMIES & FACTIONS

Before any Commander Mode battle, each side's army must be built. This
chapter covers the points economy, roster structure, and faction identity
that make two armies feel genuinely different rather than reskins of each
other.

## REQUISITION

**Requisition** is the points currency used to build an army. Every
squad's Requisition Cost can be estimated as:

> **Cost = Quality Die value (d6=2, d8=3, d10=4, d12=6) + Power + (Defense − 10) + SP + (2 × number of Traits)**

An army is built against a **Requisition Budget**, set according to Map
Size (Chapter 5):

| Map Size | Suggested Budget |
|---|---|
| 1 | 80–120 |
| 2 | 150–200 |
| 3 | 220–300 |
| 4 | 350+ |

## ROSTER ROLES

An army's budget must be spent across four roles, with minimums and
maximums enforced to prevent degenerate all-elite rosters:

| Role | Budget Share | Contains |
|---|---|---|
| **Line** | At least 40% | Levy and Regular squads |
| **Elite** | At most 30% | Veteran and Elite squads |
| **Support** | At most 25% | Volley and Siege squads |
| **Command** | Exactly 1 slot, flat cost | Signature Unit, Regiments of Renown |

## FACTION IDENTITY

Every faction that fields an army is built around three pillars.

### Doctrine

A single army-wide passive rule. Doctrines should cut both ways — a
benefit paired with a real cost — so no faction is simply "the strong one."

> ##### EXAMPLE DOCTRINES
> **Disciplined Ranks** *(disciplined/legion factions)* — Line squads gain
> +1 Defense while adjacent to another friendly Line squad.
>
> **Raiders** *(mobile/horde factions)* — All squads gain +1 Movement;
> Line squads have -1 SP.
>
> **Zealotry** *(cult/crusading factions)* — Squads automatically pass
> their first Morale save of the battle; Broken squads of this faction can
> never be targeted by a Rally order.
>
> **Siegecraft** *(engineer/fortification factions)* — Support squads cost
> 25% less Requisition; this faction cannot field a Signature cavalry unit.

### Signature Unit

A unique squad, available only to that faction, filling the Command role's
unit slot. It should do something no generic squad does — not simply be a
stronger statline.

> ##### EXAMPLE SIGNATURE UNITS
> **Revenant Guard** — Elite stats; instead of a normal Morale save, a
> Broken Revenant Guard squad returns to Full Strength at the start of its
> next turn rather than fleeing.
>
> **War Griffons** — Cavalry Movement and Charge, plus the ability to move
> over impassable terrain (rivers, walls).
>
> **Siege Titan** — Fills the entire Support role alone; devastating
> recharge attack; no Battered state — Full Strength or destroyed, nothing
> between.

### Regiments of Renown

Any squad can be **promoted** into a named Regiment for a flat Requisition
premium (+8 to +10), gaining a second trait layered atop its normal type:

| Upgrade | Effect |
|---|---|
| **Veteran Cadre** | Once per battle, reroll one failed clash or Morale save |
| **Storied Banner** | Gains the Banner/Unbreakable trait, even if its base type doesn't have it |
| **Blooded** | Gains permanent +1 Power for every battle survived and promoted in — track a running tally |
| **Personal Guard** | May be assigned to a specific officer; Orders targeting it cost 0 Command Capacity |

A Regiment that survives a battle is a natural moment to let the players
name it and choose its upgrade — this is where a campaign's army develops
history.

## REPLENISHMENT

Between War Turns, Secure Fronts generate Requisition income; Weakened
Fronts generate less; Lost Fronts generate none. Squads Broken (but not
Routed) in battle can be restored to Full Strength for half their original
Requisition cost. Routed squads are destroyed and must be rebuilt from
zero.

---

# CHAPTER 5: THE WARFRONT (COMMANDER MODE)

When player characters command an army outright, battles are resolved on
a physical hex battle map, run in structured phases rather than standard
initiative.

## MAP SIZE

Every Commander Mode battle is assigned a **Map Size** from 1 to 4,
matching the importance of the War Council Front being fought over.

| Map Size | Grid | Deployment Depth | Objectives | Terrain Features | Reserve Capacity | Fight Limit |
|---|---|---|---|---|---|---|
| **1 — Skirmish** | 6×6 | 1 hex | 1 | 1–2 | 1 squad | 2 rounds |
| **2 — Engagement** | 8×8 | 2 hexes | 1–2 | 2–3 | 2 squads | 3 rounds |
| **3 — Battle** | 10×10 | 2 hexes | 2–3 | 3–4 | 3 squads | 3 rounds |
| **4 — Siege/Decisive** | 12×12+ | 3 hexes | 3+ | 4–6 | 4+ squads | 4 rounds |

At Map Size 3, the commander gains +1 Command Capacity and +1 starting
Resources (see Chapter 6); at Map Size 4, +2 to each. At Map Size 4 only,
the per-hex stacking limit increases from 2 squads to 3.

## TERRAIN

| Terrain | Effect |
|---|---|
| Open Ground | No modifier |
| Forest/Rough | Charge traits don't function here; Volley squads can't target through it |
| Hill | +2 Defense against melee for the squad occupying it; Volley squads atop it get +2 to hit |
| River/Water | Impassable except at marked fords; attacking across a ford imposes -2 Power on the attacker |
| Fortification/Wall | +4 Defense to the defender; breached only by a Siege attack or an adjacent captured gate |
| Road | Ignore movement cost along connected road hexes |

## DEPLOYMENT

Each side deploys within its own deployment zone (set by Map Size above).
Reserve squads are set aside off-map rather than placed on a hex.

## THE BATTLEFIELD ROUND

A Warfront round proceeds through five phases, each resolved simultaneously
across the whole map before moving to the next.

**1. Command Phase.** Commanders issue Orders (below) and may play
Stratagems (Chapter 6).

**2. Movement Phase.** Every squad may move up to its Movement rating in
hexes. Both sides declare and move simultaneously.

**3. Engagement Phase.** Every hex containing squads from both sides
resolves. Melee squads (Phalanx, Charge, Skirmish) fight only what they're
adjacent to; Volley and Siege squads may fire at any target within Range
and line of sight. Each pairing is one opposed roll: **Quality Die + Power
vs. Defense**; a hit deals 1 SP, a hit beating Defense by 5+ deals 2 SP.
Unpaired squads sharing a hex add their Power as a bonus to an ally's roll
rather than rolling separately.

**4. Morale Phase.** Any squad that dropped a Condition Track step this
round makes a Morale save. A squad sharing a hex with an allied squad that
Broke this phase takes -2 on its own save.

**5. Control Phase.** Determine which side controls each hex (present,
opponent is not). Tally toward that battle's result.

> ##### FLANKING
> A squad's front faces the direction it most recently moved, or the
> enemy's deployment edge if it hasn't moved. An attack from outside that
> arc gains **+2 Power**.

## COMMAND CAPACITY & ORDERS

A commander's **Command Capacity** is 2, +1 per attached officer (an NPC or
PC assigned to relay orders), +Map Size bonuses above. Each point of
capacity issues one Order:

| Order | Effect |
|---|---|
| **Press the Attack** | Target squad: +2 Power this Engagement Phase, -2 Defense |
| **Hold the Line** | Target squad: +2 Defense this phase; cannot move this round |
| **Flank** | If sharing a hex with another attacking ally, reroll one failed clash |
| **Rally** | A Battered or Broken squad rerolls its most recent Morale save |
| **Commit Reserves** | Move a Reserve squad onto the map immediately, bypassing normal movement limits |
| **Feint** | Contested roll vs. the enemy commander (or flat DC); success grants +3 Power to one squad next round, failure Batters that squad now |

## RESOLVING THE BATTLE

Each round, tally weighted hex control (Objectives count double). When the
Fight Limit is reached, the majority holder locks the battle as Secure for
the War Council; an even split resolves as the same Pyrrhic/Stalemate
outcomes defined in Chapter 1.

---

# CHAPTER 6: RESOURCES & STRATAGEMS

Beyond Command Capacity, a faction's Doctrine grants access to
**Stratagems** — battlefield tricks fueled by a separate resource pool
representing the army's accumulated logistics and training, independent of
any one commander's personal leadership.

## RESOURCES

A commander's starting **Resources (Res)** pool equals **2 + 1 per full
100 points of Requisition spent**, plus the Map Size bonus from Chapter 5.
Resources regenerate +1 at the start of each round, capped at double the
starting value.

> ##### OPTIONAL RULE: CONVERTING LEFTOVER RESOURCES
> Unspent Resources at the end of a battle convert to Requisition for the
> next War Turn at a rate of 1 Res : 2 Requisition.

## STRATAGEM TIMING

| Tag | When It's Played |
|---|---|
| **Battle Plan** | During your own Command Phase |
| **Reactive** | During the Movement, Engagement, or Morale Phase, in direct response to an event |
| **Once per Battle** | An additional tag on high-cost effects; can't be repeated regardless of Resources available |

## UNIVERSAL STRATAGEMS

Available to every commander, regardless of faction.

| Stratagem | Cost | Timing | Effect |
|---|---|---|---|
| Forced March | 1 | Battle Plan | One squad gains +2 Movement this round |
| Steady Nerve | 1 | Reactive | One squad automatically passes its next Morale save |
| Scouted Ground | 1 | Battle Plan | One squad gains +2 on its first clash roll this round |
| Redeploy | 2 | Reactive | Move one squad up to full Movement during the Engagement Phase |
| Last Reserves | 3 (Once per Battle) | Battle Plan | Commit Reserves without spending an Order |

## DOCTRINE STRATAGEMS

> ##### DISCIPLINED RANKS
> | Stratagem | Cost | Timing | Effect |
> |---|---|---|---|
> | Shield Wall | 2 | Reactive | +4 Defense to one Line squad until your next round |
> | By the Numbers | 1 | Battle Plan | A squad that doesn't move gains +2 Power this phase |
> | Unbroken Line | 3 (Once per Battle) | Reactive | A Breaking Line squad instead holds its hex at Broken rather than fleeing |

> ##### RAIDERS
> | Stratagem | Cost | Timing | Effect |
> |---|---|---|---|
> | Lightning Raid | 2 | Battle Plan | One squad keeps its Charge bonus even if it already charged this battle |
> | Scatter and Regroup | 1 | Reactive | A Broken squad retreats to Reserve instead of being removed |
> | Howling Advance | 3 (Once per Battle) | Battle Plan | All squads: +1 Movement, +1 Power, -1 Defense this round |

> ##### ZEALOTRY
> | Stratagem | Cost | Timing | Effect |
> |---|---|---|---|
> | Martyrdom | 2 | Reactive | When a friendly squad Routs, an adjacent ally gains permanent +1 Power (stacks) |
> | Fanatical Charge | 1 | Battle Plan | One squad ignores Battered penalties this Engagement Phase |
> | The Faith Does Not Break | 3 (Once per Battle) | Reactive | A squad that failed a Morale save instead passes it and gains Banner/Unbreakable for the rest of the battle |

> ##### SIEGECRAFT
> | Stratagem | Cost | Timing | Effect |
> |---|---|---|---|
> | Overcharge the Engines | 2 | Battle Plan | A Siege squad's recharge is treated as available this round |
> | Rapid Entrenchment | 1 | Battle Plan | One squad gains Fortification's +4 Defense in open ground until it next moves |
> | Perfect the Angle | 3 (Once per Battle) | Reactive | A Siege squad's attack ignores the target's terrain-based Defense bonus |

---

# APPENDIX: QUICK REFERENCE

| System | Used When | Resolved With |
|---|---|---|
| War Council | Campaign-scale, every War Turn | Grid of Fronts, Quick Resolution, adjacency, Decisive Check |
| Squads | Any battle at any scale | Monster-style statblock, Condition Track |
| Victory Flower | PCs are Participants | Hex Flower, 2d6 Navigation Hexes |
| Warfront | PCs are Commanders | Hex battle map, 5-phase rounds |
| Requisition/Factions | Building any army | Points budget, roles, Doctrine/Signature/Regiments |
| Resources/Stratagems | Commander Mode only | Doctrine-based ability list, timing windows |

> ##### DESIGNER NOTE: SCALING THE WHOLE SYSTEM
> Every numeric dial in this supplement — Requisition Budget, Map Size,
> Heroic tier bonuses, Resources pool — is keyed either to party tier or to
> how important a given Front is to the overall war. Running this at level
> 3 and running it at level 19 should require no new rules, only larger
> numbers plugged into the same tables.