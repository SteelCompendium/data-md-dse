---
agility: 2
ancestry:
- Basilisk
- Beast
ev: '12'
file_basename: Basilisk Tonguesnapper
file_dpath: Monsters/Basilisks/Statblocks
free_strike: 4
intuition: -1
item_id: basilisk-tonguesnapper
item_index: '334'
item_name: Basilisk Tonguesnapper
level: 1
might: 1
presence: -1
reason: -3
roles:
- Elite Hexer
scc:
- mcdm.monsters.v1:monster:basilisk-tonguesnapper
scdc:
- 1.1.1:2:334
size: '2'
source: mcdm.monsters.v1
speed: 8
stability: 2
stamina: '40'
type: monster
---

```ds-statblock
name: Basilisk Tonguesnapper
level: 1
roles:
  - Elite Hexer
ancestry:
  - Basilisk
  - Beast
ev: "12"
stamina: "40"
immunities:
  - Acid 2
  - Poison 2
speed: 8
size: "2"
stability: 2
free_strike: 4
might: 1
agility: 2
reason: -3
intuition: -1
presence: -1
traits:
  - name: Petrifying Fumes
    effects:
      - effect: Any creature who starts their turn adjacent to the tonguesnapper and has
          M < 1 is slowed (save ends).
abilities:
  - name: Prehensile Tongue
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 3
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 8 acid damage; pull 1
        t2: 10 acid damage; pull 2
        t3: 14 acid damage; pull 3
      - effect: This ability can pull targets restrained by Petrifying Eye Beams, and
          ignores stability if it does so.
      - effect: The tonguesnapper targets two additional creatures or objects.
        cost: 3 Malice
  - name: Petrifying Eye Beams
    keywords:
      - Area
      - Magic
    type: Maneuver
    distance: 5 x 2 line within 1
    target: Special
    effects:
      - effect: The area extends from both the tonguesnapper's eyes, and this ability
          targets the first creature without cover on either side of the area.
        name: Special
      - roll: Power Roll + 2
        t1: A < 0 restrained (save ends)
        t2: A < 1 restrained (save ends)
        t3: Slowed (save ends); or if A < 2 restrained (save ends)
      - effect: If a target is already slowed, the potency increases by 1 for that
          target. A target restrained this way magically begins to turn to
          stone, and a target who ends two consecutive turns restrained this way
          is petrified. A target restrained this way or a creature adjacent to
          them can use a main action to cut encroaching stone from the target's
          body, dealing 8 damage to the target that can't be reduced in any way
          and ending this effect.
  - name: Wink
    cost: 2 Malice
    keywords:
      - Magic
      - Melee
      - Ranged
      - Strike
    type: Main action
    distance: Melee 1 or ranged 10
    target: One creature
    effects:
      - effect: |-
          8 corruption damage; R < 0 dazed (save ends)
          - **12-16:** 10 corruption damage; R < 1 dazed (save ends)
          - **17+:** 14 corruption damage; R < 2 dazed and slowed (save ends)
        cost: ≤11
      - effect: A creature dazed this way can't benefit from edges or double edges and
          can't gain or use surges.
  - name: Neurotoxin Splash
    keywords:
      - Area
    type: Triggered action
    distance: 2 burst
    target: Each enemy in the area
    trigger: The tonguesnapper takes damage from a melee ability.
    effects:
      - effect: Each target takes 4 acid damage. Any target who has M < 2 is also slowed
          (save ends).
```