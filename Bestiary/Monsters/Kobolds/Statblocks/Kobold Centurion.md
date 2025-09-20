---
agility: 3
ancestry:
- Kobold
- Humanoid
ev: '12'
file_basename: Kobold Centurion
file_dpath: Monsters/Kobolds/Statblocks
free_strike: 2
intuition: 0
item_id: kobold-centurion
item_index: '99'
item_name: Kobold Centurion
level: 1
might: 2
presence: 2
reason: 2
roles:
- Leader
scc:
- mcdm.monsters.v1:monster:kobold-centurion
scdc:
- 1.1.1:2:99
size: 1S
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '80'
type: monster
---

~~~ds-statblock
type: statblock
name: Kobold Centurion
level: 1
roles:
  - Leader
ancestry:
  - Kobold
  - Humanoid
ev: "12"
stamina: "80"
speed: 5
size: 1S
stability: 2
free_strike: 2
might: 2
agility: 3
reason: 2
intuition: 0
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Pilum
    icon: ⚔️
    ability_type: Signature Ability
    keywords:
      - Melee
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1 or ranged 10
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 3
        tier1: 7 damage; M < 1 weakened (save ends)
        tier2: 10 damage; M < 1 weakened (save ends)
        tier3: 13 damage; M < 1 weakened (save ends)
      - name: Effect
        effect: Each ally adjacent to a target can make a free strike against that
          target.
      - cost: 3 Malice
        effect: While weakened this way, a target is also restrained.
  - type: feature
    feature_type: ability
    name: Concentrate All Fire on That Hero!
    icon: 🏹
    keywords:
      - Ranged
    usage: Maneuver
    distance: Ranged 10
    target: One enemy
    effects:
      - name: Effect
        effect: Until the start of the centurion's next turn, the centurion and their
          allies gain an edge on power rolls against the target.
      - cost: 3+ Malice
        effect: This ability targets one additional target for each 3 Malice spent.
  - type: feature
    feature_type: ability
    name: Testudo!
    icon: ❗️
    keywords:
      - Area
    usage: Triggered action
    distance: 5 burst
    target: Each ally in the area
    trigger: A creature uses an ability that targets the centurion or an ally of the
      centurion within distance.
    effects:
      - name: Effect
        effect: Each target shifts up to 2 squares before the damage is resolved. Each
          kobold with the Shield? Shield! trait gains damage immunity 2 against
          the triggering ability.
  - type: feature
    feature_type: trait
    name: End Effect
    icon: ⭐️
    effects:
      - effect: At the end of each of their turns, the centurion can take 5 damage to
          end one effect on them that can be ended by a saving throw. This
          damage can't be reduced in any way.
  - type: feature
    feature_type: ability
    name: Firetail Pilum
    icon: ☠️
    ability_type: Villain Action 1
    keywords:
      - "-"
    usage: "-"
    distance: Special
    target: Special
    effects:
      - name: Effect
        effect: The centurion moves up to their speed, ignoring difficult terrain, and
          uses Pilum against each creature whose space they move through. They
          make one power roll against all targets, and the ability deals an
          extra 5 damage. While weakened by that ability, each target takes 2
          fire damage at the start of each of their turns.
  - type: feature
    feature_type: ability
    name: Boom Pilum!
    icon: ☠️
    ability_type: Villain Action 2
    keywords:
      - Area
      - Weapon
      - Ranged
    usage: "-"
    distance: 5 cube within 10
    target: Each enemy in the area
    effects:
      - name: Effect
        effect: The centurion uses Pilum against each target and has a double edge. Each
          target is then pushed up to 3 squares.
  - type: feature
    feature_type: ability
    name: Are You Not Entertained?!
    icon: ☠️
    ability_type: Villain Action 3
    keywords:
      - Area
    usage: "-"
    distance: 10 burst
    target: Each enemy in the area
    effects:
      - name: Effect
        effect: A target who has P < 2 is taunted (save ends). Each ally within distance
          can make a free strike. Additionally, until the end of the encounter,
          the centurion has damage immunity 2.
  - type: feature
    feature_type: trait
    name: Shield? Shield!
    icon: ⭐️
    effects:
      - effect: While adjacent to an ally who also has this trait, the centurion has
          stability 3, has cover, and grants cover to allies.
~~~