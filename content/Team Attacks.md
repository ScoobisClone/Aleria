#Rules #Homebrew 

# Overview
Sometimes, the perfect moment arises when two adventurers can synchronize their efforts into a single, devastating maneuver. This here ruleset is to introduce such an idea mechanically: team attacks, a system that turns those dramatic moments into a more formal part of your game. Team attacks require coordination, risk, and the expenditure of a shared party resource known as **Inspiration**, which has been changed from base in the [[Generic Rules#Inspiration Points|Generic Rules]]. 

# Team Action Roles and Modifiers
Each character’s class determines a team role and a team modifier, representing the kind of energy they contribute to a combined maneuver. The team modifier is an ability score modifier that gets added to attack rolls, damage, and save DCs during a team action.

|Class|Team Role|Team Modifier|
|---|---|---|
|Artificer|Defense|STR or DEX|
|Barbarian|Attack|STR|
|Bard|Healing|Spellcasting ability mod|
|Cleric|Healing|Spellcasting ability mod|
|Druid|Healing|Spellcasting ability mod|
|Fighter|Attack|STR|
|Monk|Defense|STR or DEX|
|Paladin|Defense|STR or DEX|
|Ranger|Attack|DEX|
|Rogue|Attack|DEX|
|Sorcerer|Magic|Spellcasting ability mod|
|Warlock|Magic|Spellcasting ability mod|
|Wizard|Magic|Spellcasting ability mod|

# Performing a Team Attack
A team attack is, really, a special maneuver performed by a group of characters who synchronize their actions to deliver a single strike. One character usually serves as the primary attacker, while any number of allies serve as supporters. 

### Team Attack Size and Cost
A team attack requires at least one supporter (two characters in total). There is not really a hard upper limit, but the party must spend a number of inspiration points equal to the total number of participants minus 1. The party cannot spend more points than they currently have in their pool.

## Step 1: Declare the Combination
On their turns, the primary character and all supporters can choose to participate in a team action. Every participant must be able to see the chosen target or area and be capable of taking actions. Declare which specific team action you are attempting, and ensure all requirements are met, such as role needs.

## Step 2: Take the Ready Action
Each supporter must use their action to ready their contribution. The trigger for all readied actions is "when the primary character initiates the team action." If the team action is a generic attack, the primary character prepares to make the key attack. Supporters ready the specific type of action associated with their role (a weapon attack for the Attack role, a spell for Magic role, etcetera). Spells readied in this way still require concentration and expend a spell slot as normal.

## Step 3: Resolve on the Slowest Turn
The team action resolves entirely on the turn of the participant with the lowest initiative count. That character does not need to ready and action (if they are the primary, they simply take their primary action on their turn; if they are a supporter, the use their action to ready as normal, but the team action triggers on their turn when all conditions are met). In practice, this means the action goes off when the final required participant's turn arrives and all supporters have readied actions waiting. 

If a participant is unable to take their action when the slowest turn arrives, the team action fails. No inspiration is spent, but any spell slots or abilities already committed to (such as readied spells) are lost as normal for a readied spell that did not trigger.

## Step 4: Spend Inspiration
Immediately before the team action's effects are resolved, the party must spend the required inspiration points. If the party cannot or chooses not to spend them, the team action fails: all readied actions are lost, and any spells fizzle.

# Resolving a Team Action
Once the inspiration is spent, resolve the team action as described below.

## Attack Rolls
If the team action involves an attack against a target only the primary attack rolls. If stated otherwise, all participants each roll a d20. The highest result among them is taken as the attack roll. This does not count as having advantage. Then add the team modifier of every participant to that result, even if only the primary attacker rolled.
> Example: A fighter (Attack, STR +4) and a rogue (Attack, DEX +3) perform a two-person team attack. They roll a 12 and an 18. The 18 is kept, and the total attack bonus is +7 (+4 from the fighter, +3 from the rogue), resulting in a 25 to hit.

If the team action does not involve an attack roll, skip this step.

## Damage
If the team action deals damage and is one of the special team attacks below, use the damage table below, which scales with the character level:

**Damage Table:**

| Character Level | 2 PCs | 3 PCs | 4 PCs | 5 PCs | 6 PCs  |
| --------------- | ----- | ----- | ----- | ----- | ------ |
| 1–4             | 2d10  | 3d10  | 5d10  | 8d10  | 10 d10 |
| 5–10            | 3d10  | 5d10  | 12d10 | 17d10 | 22d10  |
| 11–16           | 5d10  | 12d10 | 20d10 | 26d10 | 36d10  |
| 17–20           | 12d10 | 20d10 | 26d10 | 38d10 | 46d10  |

The damage type is determined by the weapon or spell used by the primary character, unless the team action’s description specifies otherwise. If the team action uses a saving throw for half damage, the target still takes the DT damage on a failure (half on a success), as modified by any additional effects.

Otherwise, each character is to roll their damages using their abilities as normal for a generic team attack, with the exception of adding the following to the damage roll: highest participant’s relevant ability modifier + number of participants spending inspiration.
> A fighter (Attack, STR +4), a wizard (Magic, INT +3), and a cleric (Healing, WIS +3) perform a three-person generic team attack. After hitting, each rolls normal damage. The highest ability modifier among participants is +4, and there are 3 participants spending Inspiration, so the bonus is +7. The fighter’s longsword deals 1d8 + 4 (Str) + 7, the wizard’s _fire bolt_ deals 2d10 + 7, and the cleric’s _guiding bolt_ deals 4d6 + 7.

## Saving Throws
Some team actions force one or more saving throws. The save DC is calculated using the following formula: 

Save DC = 8 + chosen participant’s relevant ability modifier with proficiency + number of participants spending inspiration

The party picks one participating character whose ability score is listed in the team action’s “Save” entry (e.g., Dexterity, Wisdom). The relevant modifier is that character’s ability modifier plus their proficiency bonus.

All creatures targeted by a team action make their saving throws with disadvantage.
> _Example:_ Two PCs, a fighter (Dex 16, +3; proficiency +2) and a wizard, attempt _Timber!_ which calls for a Dexterity save. The party uses the fighter’s stats: 8 + (3 + 2) + 2 participants = 15 DC. Goblins in the area must make a DC 15 Dexterity save at disadvantage.

# Team Attack Catalogue
Below are some team attacks that are there for anyone to use, should requirements be met. Player's that wish to create their own custom team attacks should consult with their DM and work out the details on how the attack shall work. 
Note: DT stands for Damage Table.

### Slam the Anvil
_A warrior drives an enemy onto a waiting shield, turning defense into crushing offence._
- **Participants:** 2
- **Roles:** 1 Attack, 1 Defense
- **Cost:** 1 Inspiration
- **Save:** Strength
- **Range:** Melee (primary weapon reach)
- **Duration:** Instantaneous  
    The Attack participant strikes, dealing DT bludgeoning damage. The target must then make a Strength save (DC as per rules). On a failure, it is knocked prone and its speed becomes 0 until the end of its next turn.

### Thunder Clap
_A weapon blow rings with a thunderous boom, shattering the air around the target._
- **Participants:** 2
- **Roles:** 1 Attack, 1 Magic
- **Cost:** 1 Inspiration
- **Save:** Constitution
- **Range:** Melee (primary weapon reach)
- **Duration:** Instantaneous  
    The primary attack deals DT thunder damage. Each creature of your choice within 10 feet of the target (other than the target) must make a Constitution save or take half the DT in thunder damage and be deafened until the end of its next turn. The main target also makes this save; on a failure, it takes the full DT as thunder damage and is deafened.

### Pinning Crossfire
_Two marksmen coordinate their shots to nail a foe in place._
- **Participants:** 2
- **Roles:** 2 Attack (at least one ranged weapon required)
- **Cost:** 1 Inspiration
- **Save:** None
- **Range:** 120 feet
- **Duration:** 1 round  
    Make the attack roll using the highest d20 among participants. On a hit, the target takes DT piercing damage, and its speed is reduced to 0 until the start of your next turn. A target that is Huge or larger grants advantage on the initial attack roll for participants.

### Mending Circle
_Two or more healers weave a restorative circle that mends flesh and wards against further harm._
- **Participants:** 2+
- **Roles:** 2 Healing or more
- **Cost:** 1+ Inspiration
- **Save:** None
- **Range:** 30-foot radius
- **Duration:** Instantaneous  
    Distribute a pool of hit points equal to the DT among up to six creatures of your choice within range. In addition, each creature healed gains temporary hit points equal to one of the healer's team modifiers (whoever has the highest).

### Bastion Ward
_A protector intercepts harm while essentia seals wounds preemptively._
- **Participants:** 2
- **Roles:** 1 Healing, 1 Defense
- **Cost:** 1 Inspiration
- **Save:** None
- **Range:** 30 feet
- **Duration:** 1 round  
    Choose one ally within range. That ally immediately regains hit points equal to 2 × the DT. Until the start of your next turn, the ally has resistance to all damage. During this time, whenever the ally takes damage, you may spend your reaction to reduce that damage by an amount equal to the Defense participant's team modifier + the Healing participant's team modifier (no action required).

### Brain Blast
_A guardian pins the enemy's limbs, a mage twists its mind, and a warrior delivers the silencing blow._
- **Participants:** 3
- **Roles:** 1 Attack, 1 Defense, 1 Magic
- **Cost:** 2 Inspiration
- **Save:** Wisdom
- **Range:** Melee (primary weapon reach)
- **Duration:** 1 round  
    Make the attack as normal with all participants. On a hit, the target takes DT psychic damage. It must then make a Wisdom save. On a failure, it is incapacitated until the end of its next turn. On a success, it is stunned until the end of its next turn instead. Creatures immune to psychic damage are immune to the incapacitated/stunned condition from this attack.

### Arcane Singularity
_Arcane forces converge into a swirling point of gravity that draws foes together._
- **Participants:** 3+
- **Roles:** 3 Magic or more
- **Cost:** 2+ Inspiration
- **Save:** Strength
- **Range:** 60 feet (10-foot-radius sphere)
- **Duration:** Instantaneous  
    Choose a point within range. A sphere the size of 10 x number of participants of crushing force erupts. Each creature in the area must make a Strength save. On a failure, a creature takes DT force damage and is pulled up to 20 feet toward the center of the sphere. On a success, it takes half damage and is not pulled. If a creature pulled this way ends within 5 feet of another creature, both take an additional 1d10 force damage for every other creature within 5 feet.

### Trade Offer
_A warrior's strike siphons vitality, which a healer redirects to mend allies._
- **Participants:** 3
- **Roles:** 1 Attack, 1 Magic, 1 Healing
- **Cost:** 2 Inspiration
- **Save:** None
- **Range:** Melee (primary weapon reach)
- **Duration:** Instantaneous  
    The Attack participant rolls. On a hit, the target takes DT necrotic damage (or the weapon's type, chosen by the Attack participant) plus an additional 2d10 necrotic damage. The party then chooses a number of allies within 30 feet up to the number of participants. Those allies each regain hit points equal to half the necrotic damage dealt.

### Entrenchment
_Defenders rapidly fortify a position, shielding the party behind makeshift bulwarks._
- **Participants:** 2+
- **Roles:** 2 Defense or more
- **Cost:** 1+ Inspiration
- **Save:** None
- **Range:** 30 feet
- **Duration:** 1 minute  
    Choose a square area of 10 x number of participants width on the ground within range that you can see. That area becomes difficult terrain, and creatures of your choice within it have half cover. In addition, at the moment of creation, each ally within 10 feet of that area gains temporary hit points equal to the DT.

### Judgment of the Four
_The four cardinal roles, sword, shield, spell, and spirit, unite in a gale of annihilation._
- **Participants:** 4
- **Roles:** 1 Attack, 1 Defense, 1 Magic, 1 Healing
- **Cost:** 3 Inspiration
- **Save:** Dexterity
- **Range:** Self (30-foot-radius cylinder, 60 feet high)
- **Duration:** Instantaneous  
    A roaring vortex erupts centered on the party. Each creature of your choice within the area must make a Dexterity save. A creature takes DT bludgeoning, slashing, or radiant damage (choose one type when the attack is declared) on a failure, or half as much on a success. Additionally, on a failure, the creature is pushed 20 feet away from the center and knocked prone. Huge or larger creatures have advantage on the save. After resolving, each participant can immediately move up to half their speed without provoking opportunity attacks.

# Additional Notes
- Unless otherwise stated, the team attack may only target one creature. AOE's or spells that hit multiple targets must be centered on the main target.
- Each character can only participate in a team attack once per day.



