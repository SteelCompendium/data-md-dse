---
agility: 0
ancestry:
- Elemental
- High Elf
ev: '8'
file_basename: Brambleguard
file_dpath: Monsters/Elves High/Statblocks
free_strike: 4
intuition: 0
item_id: brambleguard
item_index: '116'
item_name: Brambleguard
level: 2
might: 2
presence: 2
reason: 0
roles:
- Platoon Defender
scc:
- mcdm.monsters.v1:monster:brambleguard
scdc:
- 1.1.1:2:116
size: '2'
source: mcdm.monsters.v1
speed: 4
stability: 3
stamina: '59'
type: monster
---

~~~ds-statblock
type: statblock
name: Brambleguard
level: 2
roles:
  - Platoon Defender
ancestry:
  - Elemental
  - High Elf
ev: "8"
stamina: "59"
speed: 4
size: "2"
stability: 3
free_strike: 4
might: 2
agility: 0
reason: 0
intuition: 0
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Wall of Roses
    icon: 🔳
    ability_type: Signature Ability
    keywords:
      - Area
      - Magic
    usage: Main action
    distance: Special; see below
    target: Self
    effects:
      - name: Effect
        effect: Until the start of the brambleguard's next turn, their speed is 0 and
          they extend themself into a 5 wall. Each ally who starts their turn
          adjacent to the brambleguard regains 5 Stamina and can apply the Magic
          keyword to their weapon abilities until the end of their turn.
  - type: feature
    feature_type: ability
    name: Whip Frenzy
    icon: ❇️
    keywords:
      - Area
      - Weapon
    usage: Main action
    distance: 2 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 2
        tier1: 4 damage
        tier2: 7 damage; push 3
        tier3: 10 damage; push 3; A < 2 bleeding (save ends)
  - type: feature
    feature_type: trait
    name: Thicket and Thorns
    icon: ⭐️
    effects:
      - effect: The brambleguard blocks line of effect for enemies. Each enemy who
          starts their turn adjacent to a brambleguard takes 4 damage.
~~~