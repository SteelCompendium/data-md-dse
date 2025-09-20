---
agility: 2
ancestry:
- Undead
- Vampire
ev: '9'
file_basename: Vampire
file_dpath: Monsters/Undead/Statblocks
free_strike: 3
intuition: 1
item_id: vampire
item_index: '71'
item_name: Vampire
level: 7
might: 4
presence: 1
reason: 1
roles:
- Horde Hexer
scc:
- mcdm.monsters.v1:monster:vampire
scdc:
- 1.1.1:2:71
size: 1M
source: mcdm.monsters.v1
speed: 6
stability: 3
stamina: '40'
type: monster
---

~~~ds-statblock
type: statblock
name: Vampire
level: 7
roles:
  - Horde Hexer
ancestry:
  - Undead
  - Vampire
ev: "9"
stamina: "40"
immunities:
  - Corruption 7
  - poison 7
speed: 6
movement: Climb
size: 1M
stability: 3
free_strike: 3
might: 4
agility: 2
reason: 1
intuition: 1
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Exsanguinating Bite
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 4
        tier1: 7 damage; M < 2 bleeding (save ends)
        tier2: 10 corruption damage; M < 3 5 corruption damage and bleed- ing (save
          ends)
        tier3: 11 corruption damage; M < 4 7 corruption damage and bleeding (save ends)
      - name: Effect
        effect: The vampire regains Stamina equal to any corruption damage dealt.
  - type: feature
    feature_type: ability
    name: Vicious Pursuit
    icon: 🗡
    cost: 3 Malice
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 4
        tier1: 7 damage; A < 2 slowed (save ends)
        tier2: 10 damage; A < 3 slowed (save ends)
        tier3: 11 damage; A < 4 slowed (save ends)
      - name: Effect
        effect: If the target is bleeding, the vampire shifts up to their speed before
          using this ability.
  - type: feature
    feature_type: ability
    name: Reactive Charm
    icon: ❗️
    cost: 2 Malice
    keywords:
      - Magic
      - Ranged
    usage: Triggered action
    distance: Ranged 5
    target: One enemy
    trigger: A creature makes a strike against the vampire.
    effects:
      - name: Effect
        effect: The target becomes the new target of the strike.
  - type: feature
    feature_type: trait
    name: Unslakable Bloodthirst
    icon: ⭐️
    effects:
      - effect: The vampire has speed 10 while any creature within 10 squares of them is
          bleeding. The vampire must make a strike against a bleeding creature
          on their turn if they are able to.
~~~