---
agility: 3
ancestry:
- Undead
- Vampire
ev: '6'
file_basename: Vampire Spawn
file_dpath: Monsters/Undead/Statblocks
free_strike: 2
intuition: 1
item_id: vampire-spawn
item_index: '54'
item_name: Vampire Spawn
level: 4
might: 2
presence: 2
reason: -1
roles:
- Horde Harrier
scc:
- mcdm.monsters.v1:monster:vampire-spawn
scdc:
- 1.1.1:2:54
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '30'
type: monster
---

~~~ds-statblock
type: statblock
name: Vampire Spawn
level: 4
roles:
  - Horde Harrier
ancestry:
  - Undead
  - Vampire
ev: "6"
stamina: "30"
immunities:
  - Corruption 4
  - poison 4
speed: 5
movement: Climb
size: 1M
stability: 0
free_strike: 2
might: 2
agility: 3
reason: -1
intuition: 1
presence: 2
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
      - roll: Power Roll + 3
        tier1: 5 damage
        tier2: 7 corruption damage; M < 2 bleeding (save ends)
        tier3: 9 corruption damage; M < 3 bleeding (save ends)
      - name: Effect
        effect: The vampire spawn regains Stamina equal to any corruption damage dealt.
      - cost: 1 Malice
        effect: The target takes an additional 3 corruption damage.
  - type: feature
    feature_type: ability
    name: Vampiric Celerity
    icon: 👤
    keywords:
      - "-"
    usage: Maneuver
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The vampire spawn can shift 1 square, then move up to their speed. The
          next ability the vampire uses before the start of their next turn
          gains an edge.
  - type: feature
    feature_type: trait
    name: Unslakable Bloodthirst
    icon: ⭐️
    effects:
      - effect: The vampire spawn has speed 10 while any creature within 10 squares of
          them is bleeding. The vampire spawn must use Exsanguinating Bite
          against a bleeding creature on their turn if they are able to.
~~~