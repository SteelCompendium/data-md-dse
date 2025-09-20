---
agility: 0
ancestry:
- Basilisk
- Beast
ev: '12'
file_basename: Basilisk
file_dpath: Monsters/Basilisks/Statblocks
free_strike: 5
intuition: -1
item_id: basilisk
item_index: '333'
item_name: Basilisk
level: 1
might: 2
presence: -1
reason: -3
roles:
- Elite Brute
scc:
- mcdm.monsters.v1:monster:basilisk
scdc:
- 1.1.1:2:333
size: '2'
source: mcdm.monsters.v1
speed: 8
stability: 2
stamina: '80'
type: monster
---

~~~ds-statblock
type: statblock
name: Basilisk
level: 1
roles:
  - Elite Brute
ancestry:
  - Basilisk
  - Beast
ev: "12"
stamina: "80"
immunities:
  - Poison 4
speed: 8
size: "2"
stability: 2
free_strike: 5
might: 2
agility: 0
reason: -3
intuition: -1
presence: -1
features:
  - type: feature
    feature_type: ability
    name: Noxious Bite
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main Action
    distance: Melee 1
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        tier1: 7 poison damage
        tier2: 10 poison damage
        tier3: 13 poison damage
      - name: Effect
        effect: This ability gains an edge against targets the basilisk has previously
          dealt poison damage to.
  - type: feature
    feature_type: ability
    name: Petrifying Eye Beams
    icon: 🔳
    keywords:
      - Area
      - Magic
    usage: Maneuver
    distance: 5 x 2 line within 1
    target: Special
    effects:
      - name: Special
        effect: The area extends from both the basilisk's eyes, and this ability targets
          the first creature without cover on either side of the area.
      - roll: Power Roll + 2
        tier1: M < 0 restrained (save ends)
        tier2: M < 1 restrained (save ends)
        tier3: Slowed (save ends); or if M < 2 restrained (save ends)
      - name: Effect
        effect: If a target is already slowed, the potency increases by 1 for that
          target. A target restrained this way magically begins to turn to
          stone, and a target who ends two consecutive turns restrained this way
          is petrified. A target restrained this way or a creature adjacent to
          them can use a main action to cut encroaching stone from the target's
          body, dealing 8 damage to the target that can't be reduced in any way
          and ending this effect.
  - type: feature
    feature_type: ability
    name: Poison Fumes
    icon: 🔳
    cost: 5 Malice
    keywords:
      - Area
      - Magic
    usage: Main action
    distance: 3 cube within 1
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 2
        tier1: 4 poison damage; M < 0 weakened (save ends)
        tier2: 6 poison damage; M < 1 weakened and slowed (save ends)
        tier3: 9 poison damage; M < 2 weakened and slowed (save ends)
  - type: feature
    feature_type: ability
    name: Lash Out
    icon: ❗️
    keywords:
      - Area
    usage: Triggered action
    distance: 1 burst
    target: Each enemy in the area
    trigger: The basilisk takes damage from a melee ability.
    effects:
      - name: Effect
        effect: Each target takes 5 damage. Any target who has A < 2 is also bleeding
          (save ends).
  - type: feature
    feature_type: trait
    name: Calcifying Presence
    icon: ⭐️
    effects:
      - effect: The area within 3 squares of the basilisk is difficult terrain for
          enemies.
~~~