#Rules #Homebrew 
# Modularity in Armor and Damage
This system treats armor as a collection of modular pieces. Protection Rating (PR) represents the overall amount of armor worn, while armor category determines how that protection is expressed:
- Light armor favors evasion: Dexterity contributes fully to AC, but DR is lower.
- Medium armor provides a balanced approach, with a limited Dexterity bonus and no category adjustment to DR.
- Heavy armor favors absorption: it limits Dexterity, reduces AC slightly, and increases DR.
- Weapon properties such as Heavy Impact and Precise give attackers ways to challenge armor without making armor universally ineffective.

This system also remains abstract (attacks do not target individual armor slots) as to stay in line with base DnD.

## Armor Pieces
You have five armor slots: Head, Torso, Arms, Legs, and Feet. You may wear one piece in each slot. Each piece has a Protection Rating (PR), weight, category tag, and possibly a special property.

| Slot | Item | PR | Weight | Category | Special |
|---|---|---:|---:|---|---|
| Head | Full Helm | 5 | 5 lb | Heavy | — |
| Head | Half Helm | 4 | 3 lb | Medium | — |
| Head | Chainmail Cowl | 3 | 2 lb | Light | +2 DR vs. slashing, -2 DR vs. bludgeoning |
| Head | Padded Coif | 2 | 1 lb | Light | — |
| Torso | Breastplate | 5 | 18 lb | Medium | — |
| Torso | Chainmail Hauberk | 4 | 16 lb | Medium | +2 DR vs. slashing, -2 DR vs. bludgeoning |
| Torso | Leather Jerkin | 3 | 10 lb | Light | — |
| Torso | Padded Gambeson | 2 | 8 lb | Light | — |
| Arms | Plate Gauntlets | 4 | 5 lb | Heavy | — |
| Arms | Splint Vambraces | 3 | 4 lb | Medium | — |
| Arms | Chain Gauntlets | 2 | 3 lb | Light | +1 DR vs. slashing |
| Arms | Leather Gloves | 1 | 2 lb | Light | — |
| Legs | Plate Leggings | 5 | 18 lb | Heavy | — |
| Legs | Splint Leggings | 4 | 14 lb | Medium | — |
| Legs | Chain Skirt | 3 | 12 lb | Light | +1 DR vs. slashing |
| Legs | Gambeson Pants | 2 | 6 lb | Light | — |
| Feet | Plate Greaves | 3 | 7 lb | Heavy | — |
| Feet | Splint Greaves | 2 | 5 lb | Medium | — |
| Feet | Leather Boots | 1 | 3 lb | Light | — |
**Special:** Piece-specific damage modifiers apply to DR after the armor category modifier. Modifiers stack unless otherwise stated.

### Total Protection Rating
Your total PR is the sum of the PR from every occupied slot:
`Total PR = Head + Torso + Arms + Legs + Feet`
An empty slot contributes 0 PR unless an item or feature states otherwise.

Example: Full Helm (5) + Breastplate (5) + Plate Gauntlets (4) + Plate Leggings (5) + Plate Greaves (3) = 22 PR.

## From PR to Base AC and Base DR
Look up total PR on the table below. PR determines both Base AC and Base DR before Dexterity, armor category, or special modifiers are applied.

| Total PR | Base AC | Base DR |
|---:|---:|---:|
| 0–6 | 10 | 0 |
| 7–8 | 11 | 1 |
| 9–10 | 12 | 2 |
| 11–12 | 13 | 3 |
| 13–14 | 14 | 4 |
| 15–16 | 15 | 5 |
| 17–18 | 16 | 6 |
| 19–20 | 17 | 7 |
| 21+ | 18 | 8 |

Beyond 21 PR, calculate Base AC and Base DR using these formulas:
- `Base AC = 18 + floor((PR - 21) / 2)`
- `Base DR = 8 + floor((PR - 21) / 3)`
Always round down. If a character's total PR is 21 or lower, use the table.

---

## Armor Categories
Each armor piece has a category: Light, Medium, or Heavy. When wearing multiple pieces, use the most restrictive category among all worn pieces to determine Dexterity limits, the category AC modifier, the category DR modifier, and stealth effects.

| Category | Dexterity Bonus to AC | Category AC Modifier | Category DR Modifier | Stealth |
|---|---|---:|---:|---|
| Light | Full Dexterity modifier | +0 | -2 | Normal |
| Medium | Maximum +2 | +0 | +0 | Normal |
| Heavy | +0 | -1 | +2 | Disadvantage |
A character wearing any Heavy piece uses the Heavy category. Otherwise, a character wearing any Medium piece uses Medium. A character wearing only Light pieces uses Light.

### Final AC
`Final AC = Base AC + allowed Dexterity modifier + category AC modifier + other applicable bonuses`

For example, a character with 17 PR has Base AC 16. If the character has Dexterity 18 (+4) and wears only Light armor, their AC is 16 + 4 + 0 = 20.

If the same character wears Medium armor, their Dexterity bonus is capped at +2, so their AC is 16 + 2 + 0 = 18.

If the same character wears Heavy armor, they add no Dexterity and apply the -1 category modifier, so their AC is 16 + 0 - 1 = 15.

### Final DR
`Final DR = Base DR + category DR modifier + piece-specific DR modifiers`

DR cannot be reduced below 0 before it is applied to damage.

Example: A character has 17 PR (Base DR 6) and wears Heavy armor (+2 category DR). They also wear a Chainmail Hauberk with +2 DR vs. slashing and -2 DR vs. bludgeoning.
- DR vs. slashing = 6 + 2 + 2 = 10
- DR vs. bludgeoning = 6 + 2 - 2 = 6
- DR vs. piercing = 6 + 2 = 8

## Damage Reduction in Detail
When a creature takes bludgeoning, piercing, or slashing damage from an attack, subtract its applicable DR from the damage.
- Damage cannot be reduced below 1 by DR.
- By default, DR applies only to bludgeoning, piercing, and slashing damage.
- Apply category and piece-specific DR modifiers before reducing the damage.
- DR applies separately to each qualifying hit.
- Resistance, vulnerability, and other damage adjustments are applied according to the campaign's chosen 5e damage-resolution order. The DM should use one consistent order throughout the campaign. For the sake of my campaigns, I will be using DR first and foremost.
Example: A character has 8 DR and is hit by three attacks that each deal 6 slashing damage. Each hit deals at least 1 damage after DR, so the character takes 3 damage total.

## Weapon Properties
Some weapons and attacks have properties designed to challenge armor. These properties affect DR, not AC, unless an ability explicitly says otherwise.

### Heavy Impact / Precise
A Heavy Impact attack is especially forceful and can overwhelm armor.

**Heavy Impact / Precise (X):** Reduce the target's applicable DR by X against this attack, to a minimum of 0, before subtracting DR from the damage.

### Property Limits
- Heavy Impact and Precise do not stack with each other on the same attack. If an attack has both properties, it ignores DR based on the higher one.
- These properties do not lower AC or guarantee a hit.
- Apply the property after determining the target's applicable DR from Base DR, category, and armor-piece modifiers.
- DR ignored by a property cannot become negative.
- Unless an item or feature says otherwise, these properties apply only to the attack that has the property.

Example: A Heavy armor character has 8 DR against a slashing attack. A weapon with Heavy Impact reduces the effective DR to 6 for that attack. If the attack deals 15 slashing damage, the character takes 9 damage.

## Shields
A shield is a separate defensive item and does not occupy one of the five armor slots or contribute PR by default.

Unless a shield's description says otherwise, it grants its normal 5e AC bonus. It does not increase DR.

## Class Features, Natural Armor, and Magic
Use the following guidelines to avoid stacking incompatible AC calculations:
- **Unarmored Defense:** Use the feature's AC calculation instead of the armor-based AC calculation, unless a feature explicitly allows them to combine. A character using Unarmored Defense does not gain armor category modifiers from worn armor.
- **Natural Armor:** Treat natural armor as an alternative AC calculation when the feature says it sets a character's AC. Follow the feature's own wording.
- **Mage Armor:** Treat Mage Armor as an alternative AC calculation as written. It does not add to armor-based AC.
- **Magic armor:** A magic bonus to AC applies to Final AC if the item's description says it does. A bonus to PR increases PR only if the item's description explicitly grants PR.
- **Other DR or resistance:** Apply according to the specific feature's wording and the DM's consistent damage-resolution order. Do not assume separate DR effects stack unless their descriptions allow it.
When an ability or magic item conflicts with these general guidelines, its specific wording takes precedence.

## Standard D&D Armor Converted Over

| Standard Armor | Total PR | Base AC | Base DR | Category | Strength Requirement |
|---|---:|---:|---:|---|---|
| Padded | 7 | 11 | 1 | Light | — |
| Leather | 8 | 11 | 1 | Light | — |
| Studded Leather | 10 | 12 | 2 | Light | — |
| Hide | 11 | 13 | 3 | Medium | — |
| Chain Shirt | 12 | 13 | 3 | Medium | — |
| Scale Mail | 13 | 14 | 4 | Medium | — |
| Breastplate | 14 | 14 | 4 | Medium | — |
| Half Plate | 16 | 15 | 5 | Medium | — |
| Ring Mail | 15 | 15 | 5 | Heavy | Str 13 |
| Chain Mail | 17 | 16 | 6 | Heavy | Str 13 |
| Splint | 19 | 17 | 7 | Heavy | Str 14 |
| Plate | 22 | 18 | 8 | Heavy | Str 15 |

These conversion totals assume typical combinations of modular pieces. For example, Plate may include a Full Helm, Breastplate, Plate Gauntlets, Plate Leggings, and Plate Greaves. The DM may allow substitutions while retaining the listed total PR, if appropriate for the campaign.

**Important:** When using my modular armor rules, calculate AC and DR from the character's actual worn pieces and total PR. Do not add the standard armor's listed Base AC or Base DR on top of the calculated values.
