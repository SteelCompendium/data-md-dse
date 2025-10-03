---
agility: 3
ancestry:
- Horror
- Voiceless Talker
ev: '32'
file_basename: Mindkiller
file_dpath: Monsters/Voiceless Talkers/Statblocks
free_strike: 7
intuition: 2
item_id: mindkiller
item_index: '338'
item_name: Mindkiller
level: 6
might: -1
presence: 0
reason: 3
roles:
- Elite Hexer
scc:
- mcdm.monsters.v1:monster:mindkiller
scdc:
- 1.1.1:2:338
size: 1S
source: mcdm.monsters.v1
speed: 6
stability: 2
stamina: '140'
type: monster
---

~~~ds-statblock
type: statblock
name: Mindkiller
level: 6
roles:
  - Elite Hexer
ancestry:
  - Horror
  - Voiceless Talker
ev: "32"
stamina: "140"
immunities:
  - Psychic 6
speed: 6
movement: Fly, hover
size: 1S
stability: 2
free_strike: 7
might: -1
agility: 3
reason: 3
intuition: 2
presence: 0
features:
  - type: feature
    feature_type: trait
    name: Brain Latch
    icon: ⭐️
    effects:
      - effect: The mindkiller can grab creatures who are size 4 or smaller, using their
          Reason score in place of Might. A creature grabbed by the mindkiller
          takes a bane on ability rolls made to escape the grab.
  - type: feature
    feature_type: ability
    name: Killer Claws
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
        tier1: 11 damage
        tier2: 17 damage; A < 2 grabbed
        tier3: 21 damage; A < 3 grabbed
  - type: feature
    feature_type: ability
    name: Concealing Strike
    icon: 🏹
    cost: 2 Malice
    keywords:
      - Psionic
      - Ranged
      - Strike
    usage: Main action
    distance: Ranged 5
    target: Two creatures
    effects:
      - roll: Power Roll + 3
        tier1: 10 damage; R < 1 the mindkiller is invisible to the target (save ends)
        tier2: 15 damage; R < 2 the mindkiller is invisible to the target (save ends)
        tier3: 18 damage; R < 3 the mindkiller is invisible to the target (save ends)
  - type: feature
    feature_type: ability
    name: Mindwipe
    icon: 🗡
    keywords:
      - Melee
      - Psionic
      - Strike
    usage: Maneuver
    distance: Melee 1
    target: One creature
    effects:
      - name: Effect
        effect: The target must be grabbed by the mindkiller. If the target has R < 2,
          they take a −1 penalty to their Reason, Intuition, or Presence score
          and the mindkiller has a +1 bonus to the same score, all until the end
          of the encounter.
  - type: feature
    feature_type: ability
    name: Meat Shield
    icon: ❗️
    keywords:
      - "-"
    usage: Triggered action
    distance: Self
    target: Self
    trigger: The mindkiller takes damage.
    effects:
      - name: Effect
        effect: The mindkiller halves the damage. If the mindkiller has a creature
          grabbed, that creature takes the other half of the damage.
      - cost: 3 Malice
        effect: A grabbed creature takes the damage instead of the mindkiller.
  - type: feature
    feature_type: trait
    name: Psionic Conductor
    icon: ⭐️
    effects:
      - effect: Whenever a non-minion voiceless talker within 5 squares of the
          mindkiller uses a psionic ability, they can do so as if they were in
          the mindkiller's space.
  - type: feature
    feature_type: trait
    name: Nimble
    icon: ⭐️
    effects:
      - effect: The mindkiller can move through enemies' spaces at their usual speed.
~~~