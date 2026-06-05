---
title: Resolve & Mental Exhaustion
---
#Rules #Homebrew 
# Resolve Points (RP)
Every character has a maximum number of Resolve Points, calculated as follows: 
`RP Max = 2 * (10 + Level + Highest Mental Score)`
Example: A 5th-level character with Wisdom 16 has an RP Max = 2 * (10 + 5 + 16) = 62.

Resolve Points are tracked like hit points and are handled on Foundry.

## Gaining RP Examples
- Enemy Takedown. When you reduce a hostile creature to 0 hit points, you regain 5 RP.
- Combat End. When initiative ends, you regain 8 + your Wisdom modifier RP (minimum 1).
- Unpanicking an Ally. As an action, you may make a Wisdom (Insight) check (DC = 10 + the panicked ally's level). On success, the ally's Panic is reduced to Stress, and you both regain 5 RP.
- Other Means. The DM (Which is me) may award RP for achieving narrative goals, resting in safety, or receiving magical means of mental help.
## Losing RP Examples
- Pressure. When you enter combat against a creature whose CR is 4 or more higher than your level, you lose 5 + 2 RP per point difference (Maximum 20 RP).
- Staggered. When you are reduced to 0 hit points, you lose 10 RP.
- Bleed Out. When an ally within 30 feet drops to 0 hit points, you lose 8 RP (once per ally per combat).
- Other Stressors. The DM may call for RP loss due to horrifying sights, psychological manipulation, or extended duress.
$_{\text{This is all up to DM (which means my) choice and are not necessarily hard rules of this system.}}$

---

# Resolve Thresholds
Your current RP determines your mental state.

|State|RP Range|Description|
|---|---|---|
|**Normal**|> 50% of RPmax|You are composed and in control.|
|**Stressed**|≤ 50% of RPmax|You are strained; your behavior starts to shift.|
|**Panic**|≤ 10% of RPmax|Your mind breaks; you lose control.|
## Stress
When your RP first drops to less than 50% of your RP Max during combat, you immediately become **Stressed**. Roll 1d4 to determine your **Stress Type**. The type remains until you clear the Stress condition detailed further below.

While Stressed, you gain the **Stress Effect** associated with your type as well as 1 level of **Mental Exhaustion** at the end of combat. This Mental Exhaustion only goes up to level 3.
> **Re-entering Stress.** If your RP later rises above 50% and then falls again, you roll a new Stress Type. If you were already Stressed and your RP remains below or equal to 50%, your type does not change.

### Ending Stress
Stress ends only when your RP rises above 90% of RP Max. Until then, you remain Stressed (This can carry over from one combat to the next if you do not recover enough RP).

## Panic
When your RP drops equal to or below 10% of RP Max, you immediately Panic:
1. Gain 1 level of Mental Exhaustion immediately (this replaces the one you would have gained from Stress). This Mental Exhaustion only goes up to level 3.
2. Your current Stress Type determines your **Panic Effect** and **Panic Behavior**. If you somehow were not Stressed when Panic occurs, roll randomly on the Stress Type table.
3. The Panic Effect replaces your Stress Effect for as long as you are Panicking.
4. You are unable to cast spells or use features that require concentration/mental focus.
5. It is impossible for you to regain RP the turn you become Panicked.

While Panicking, you cannot choose your own actions completely freely. On each of your turns, you must follow the Panic Behavior dictated by your type.
> **Multiple Panics.** If you recover from Panic and later drop to ≤10% RP again, you do not gain another level of Mental Exhaustion and re-enter Panic. You may roll a new Stress Type if you are no longer Stressed; otherwise, use your current type.

### Ending Panic
Panic ends automatically when your RP rises above 50% of RP Max. No other condition ends Panic.

---

# Resolve Effects Table

| Type       | Stress Effect (RP ≤ 50%)                                                                                 | Panic Effect (RP ≤ 10%)                                                                                              | Panic Behavior (each turn)                                                                                                                                                                                                                   |
| ---------- | -------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Fight**  | AC –2, attack rolls +2                                                                                   | AC –4, attack rolls +4                                                                                               | Move adjacent to the nearest creature (random if tie). Use your action(s) to Attack the nearest target (can be an ally).                                                                                                                     |
| **Flight** | Speed +10 ft, opportunity attacks against you have advantage                                             | Speed +30 ft, opportunity attacks against you have advantage and deal an extra 1d6 damage                            | Take the Disengage action, then move as far as possible from all enemies (through hazards if necessary). Use any remaining actions to Dash.                                                                                                  |
| **Fawn**   | Help action grants ally +1d4 on next attack; you have disadvantage on saving throws until your next turn | Help action grants ally +2d4 on next attack; enemies have advantage on attack rolls against you until your next turn | Move adjacent to the nearest creature (random if tie). Take the Dodge  or Help action. Convert any remaining actions into Reactions; you must use your Reaction to intercept attacks against any creature within 5 feet (including enemies). |
| **Freeze** | AC +2, speed halved                                                                                      | AC +4, speed 0                                                                                                       | You cannot move. Convert your action(s) into Reactions. You cannot make opportunity attacks.                                                                                                                                                 |
# Custom Stress Types
The four core Stress Types (Fight, Flight, Fawn, Freeze) cover most situations, but the DM or abilities may introduce custom Stress Types. A custom Stress Type has its own Stress Effect, Panic Effect, and Panic Behavior, created using the existing ones as a template. 

## Rules for Custom Stress Types
- **Override Priority.** When a character would gain a Stress Type from any source, the newest type always overrides the current one. This applies regardless of whether the new type comes from the core table or a custom type. 
- **Multiple Overrides.** If a character already has a custom Stress Type and then gains another custom Stress Type, the most recently gained type takes effect.
- **Duration.** Custom Stress Types follow the same rules for ending Stress and for Panic. They do not persist longer than normal unless specified, but they can persist shorter than usual when specified.

## Examples of Custom Stress Types

| Name         | Stress Effect (RP ≤ 50%)                                                                                                                                 | Panic Effect (RP ≤ 10%)                                                                                                                                       | Panic Behavior (each turn)                                                                                                                   |
| ------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| **Haunted**  | You hear whispers. You have disadvantage on Perception checks, but gain +2 on Insight checks.                                                            | The whispers become screams. You cannot hear any sound. You are deafened.                                                                                     | You must move away from all light sources. If in darkness, you stand still and cannot take actions.                                          |
| **Obsessed** | You fixate on one enemy (choose when Stress starts). Attack rolls against that enemy have advantage; attack rolls against anyone else have disadvantage. | You ignore all other enemies. You will not attack or defend against anyone except your fixation. You gain a bonus +4 for hits and damage against your target. | You must use your action to Dash toward your fixated enemy. If already adjacent, you attack them and only them.                              |
| **Giddy**    | You laugh uncontrollably. You have advantage on Charisma (Performance) checks but disadvantage on Dexterity saves.                                       | You collapse into hysterical laughter. You are prone and cannot stand.                                                                                        | On your turn, you must use your action to laugh. You cannot take reactions or move more than 5 feet.                                         |
| **Weeping**  | You cry constantly. Allies within 10 feet have advantage on Wisdom saves, but you have disadvantage on attack rolls.                                     | You sob uncontrollably. You cannot speak or cast spells with verbal components.                                                                               | You must move toward the nearest ally and take the Help action to assist them (including cleaning their visor, handing them a weapon, etc.). |

## Custom Types and Panic
When a character with a custom Stress Type drops to ≤10% RP, they Panic using that custom type’s Panic Effect and Behavior. If the custom type has no defined Panic entry, default to the nearest core type (at the DM's discretion).

---

# Mental Exhaustion
Intense mental activities such as studying, deciphering, solving a problem that takes longer than an hour, may inflict a level of Mental Exhaustion. This counts as a type of Exhaustion and is tracked separately from normal Exhaustion. Effects that lower Exhaustion also lower Mental Exhaustion by the same number of levels in the same way.

Similar to regular Exhaustion, the first three levels are soft exhaustion and the final three are heavy exhaustion. As such, these levels also follow about the same rules that normal exhaustion undergoes.

## Mental Exhaustion Table

| Level | DC  | Effect                                                                                                                                                                                         |
| ----- | --- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1     | –   | Disadvantage on Intelligence, Wisdom and Charisma checks                                                                                                                                       |
| 2     | –   | Speed of mental activity halved. You feel sleepy, and may ignore fine detail.                                                                                                                  |
| 3     | 15  | Speed of mental activity halved again. Disadvantage on Intelligence, Wisdom and Charisma saving throws. You barely maintain your focus on the subject of your study, and ignore anything else. |

#### Soft Mental Exhaustion

| Level | Ignore DC | Effect                                                                                                                                                            |
| ----- | --------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1     | –         | Disadvantage on Intelligence, Wisdom, and Charisma ability and skill checks.                                                                                      |
| 2     | –         | Disadvantage on all mental ability and skill checks (Int/Wis/Cha). You feel foggy; speed of mental tasks halved (e.g., reading, deciphering takes twice as long). |
| 3     | 15        | Disadvantage on Intelligence, Wisdom, and Charisma saving throws.                                                                                                 |

#### Heavy Mental Exhaustion

| Level | Ignore DC | Effect                                                                                                                                                                                                                                 |
| ----- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 4     | 18        | You can only concentrate on one thing at a time (e.g., one spell, one enemy). You ignore all other sensory input. You cannot perform tasks requiring multi-step reasoning (e.g., solving a puzzle, ritual casting).                    |
| 5     | 20        | You cannot concentrate on spells or abilities requiring concentration. You suffer from hallucinations, tunnel vision, or vertigo (GM chooses). You cannot cast spells above 3rd level.                                                 |
| 6     | 25        | You are broken. You cannot take any action that requires a decision. You can only perform reflexive actions (e.g., move away from danger, dodge). Any additional level of Mental Exhaustion causes you to fall unconscious for 1 hour. |

#### Ignoring Mental Exhaustion
When you attempt an action that would increase your Mental Exhaustion to a level with an Ignore DC (levels 3, 4, 5, 6), you must make a **Wisdom saving throw** against that DC. On a success, you ignore the exhaustion and perform the action; on a failure, you find an excuse not to do it (you cannot attempt the same action for 1 minute).

#### Excess Soft Mental Exhaustion
If you are already at level 3 (Soft maximum) and would gain another level of Mental Exhaustion from a Soft source (e.g., post-combat stress while already at level 3), instead of increasing to level 4, you lose one spell slot/equivalent feature starting from your lowest. If you have no spell slots/equivalent feature left, your Mental Exhaustion increases to level 4 as normal.



