---
agility: 3
ancestry:
- Beast
- Wyvern
ev: '24'
file_basename: Wyvern Lurker
file_dpath: Monsters/Wyverns/Statblocks
free_strike: 6
intuition: 1
item_id: wyvern-lurker
item_index: '121'
item_name: Wyvern Lurker
level: 4
might: 2
presence: 0
reason: -1
roles:
- Elite Ambusher
scc:
- mcdm.monsters.v1:monster:wyvern-lurker
scdc:
- 1.1.1:2:121
size: '2'
source: mcdm.monsters.v1
speed: 9
stability: 2
stamina: '120'
type: monster
---

~~~ds-statblock
type: statblock
name: Wyvern Lurker
level: 4
roles:
  - Elite Ambusher
ancestry:
  - Beast
  - Wyvern
ev: "24"
stamina: "120"
immunities:
  - Acid 5
speed: 9
movement: Fly
size: "2"
stability: 2
free_strike: 6
might: 2
agility: 3
reason: -1
intuition: 1
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Agonizing Stinger
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Magic
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 2
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 3
        tier1: 9 damage
        tier2: 14 damage; M < 2 bleeding (save ends)
        tier3: 17 damage; M < 3 bleeding (save ends)
      - cost: 1 Malice
        effect: One target hidden from the lurker takes an extra 6 acid damage.
  - type: feature
    feature_type: ability
    name: Acidic Anguish
    icon: 🗡
    cost: 3 Malice
    keywords:
      - Magic
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 2
    target: One creature or object
    effects:
      - roll: Power Roll + 3
        tier1: 10 acid damage; M < 1 weakened (save ends)
        tier2: 16 acid damage; M < 2 weakened (save ends)
        tier3: 20 acid damage; M < 3 weakened (save ends)
      - name: Effect
        effect: A target weakened this way takes 1d4 acid damage at the start of each of
          their turns.
  - type: feature
    feature_type: ability
    name: Swooping Torment
    icon: 👤
    keywords:
      - "-"
    usage: Maneuver
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The lurker flies up to their speed, then can attempt to hide. Each enemy
          the lurker moves adjacent to during this movement can choose to take 3
          sonic damage or fall prone.
  - type: feature
    feature_type: ability
    name: Retaliatory Dive
    icon: ❗️
    keywords:
      - Ranged
    usage: Triggered action
    distance: Ranged 5
    target: The triggering creature
    trigger: A creature within distance deals damage to the lurker with a ranged
      ability.
    effects:
      - name: Effect
        effect: The lurker flies adjacent to the target and can make a free strike
          against them.
  - type: feature
    feature_type: trait
    name: Ruthless Rage
    icon: ⭐️
    effects:
      - effect: While within 10 squares of another wyvern, the lurker deals an extra 3
          damage with strikes.
  - type: feature
    feature_type: trait
    name: Tenacious Hunter
    icon: ⭐️
    effects:
      - effect: Any creature affected by a condition imposed by a wyvern can't be hidden
          from the lurker.
~~~