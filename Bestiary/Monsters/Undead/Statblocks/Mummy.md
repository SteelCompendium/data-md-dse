---
agility: -1
ancestry:
- Mummy
- Undead
ev: '6'
file_basename: Mummy
file_dpath: Monsters/Undead/Statblocks
free_strike: 3
intuition: 3
item_id: mummy
item_index: '61'
item_name: Mummy
level: 4
might: 3
presence: 0
reason: 1
roles:
- Horde Brute
scc:
- mcdm.monsters.v1:monster:mummy
scdc:
- 1.1.1:2:61
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '50'
type: monster
---

~~~ds-statblock
type: statblock
name: Mummy
level: 4
roles:
  - Horde Brute
ancestry:
  - Mummy
  - Undead
ev: "6"
stamina: "50"
immunities:
  - Corruption 4
  - poison 4
weaknesses:
  - Fire 5
speed: 5
size: 1M
stability: 2
free_strike: 3
might: 3
agility: -1
reason: 1
intuition: 3
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Accursed Bindings
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 3
    target: One creature or object
    effects:
      - roll: Power Roll + 3
        tier1: 6 corruption damage; pull 1
        tier2: 8 corruption damage; pull 2
        tier3: 10 corruption damage; pull 2; M < 3 restrained (save ends)
      - name: Effect
        effect: The next ability the mummy uses against the target has any potency
          increased by 1 for the target.
  - type: feature
    feature_type: ability
    name: Eldritch Curse
    icon: 🏹
    cost: 3 Malice
    keywords:
      - Magic
      - Ranged
    usage: Main action
    distance: Ranged 10
    target: One creature
    effects:
      - roll: Power Roll + 3
        tier1: 3 corruption damage; I < 1 the target is cursed (save ends)
        tier2: 5 corruption damage; I < 2 the target is cursed (save ends)
        tier3: 7 corruption damage; I < 3 the target is cursed (save ends)
      - name: Effect
        effect: A cursed target is bleeding and weakened, and allies gain an edge on
          strikes made against them.
  - type: feature
    feature_type: ability
    name: Blast of Mummy Dust
    icon: ❗️
    cost: 1 Malice
    keywords:
      - Area
    usage: Triggered action
    distance: 1 burst
    target: The triggering creature
    trigger: The mummy comes within distance of a restrained creature or starts
      their turn within distance of one.
    effects:
      - name: Effect
        effect: The target takes 8 poison damage.
~~~