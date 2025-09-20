---
agility: 3
ancestry:
- Beast
- Manticore
ev: '72'
file_basename: Manticore
file_dpath: Monsters/Manticores/Statblocks
free_strike: 6
intuition: 0
item_id: manticore
item_index: '348'
item_name: Manticore
level: 4
might: 4
presence: -1
reason: 0
roles:
- Solo
scc:
- mcdm.monsters.v1:monster:manticore
scdc:
- 1.1.1:2:348
size: '2'
source: mcdm.monsters.v1
speed: 10
stability: 2
stamina: '350'
type: monster
---

~~~ds-statblock
type: statblock
name: Manticore
level: 4
roles:
  - Solo
ancestry:
  - Beast
  - Manticore
ev: "72"
stamina: "350"
speed: 10
movement: Fly
size: "2"
stability: 2
free_strike: 6
might: 4
agility: 3
reason: 0
intuition: 0
presence: -1
features:
  - type: feature
    feature_type: trait
    name: Solo Monster
    icon: ☠️
    effects:
      - name: End Effect
        effect: At the end of each of their turns, the manticore can take 10 damage to
          end one effect on them that can be ended by a saving throw. This
          damage can't be reduced in any way.
      - name: Solo Turns
        effect: The manticore can take two turns each round. They can't take turns
          consecutively.
  - type: feature
    feature_type: trait
    name: Agile Predator
    icon: ⭐️
    effects:
      - effect: Whenever the manticore deals damage to a creature, they don't provoke
          opportunity attacks from that creature during that turn.
  - type: feature
    feature_type: ability
    name: Carnivorous Bite
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
        tier1: 12 damage; A < 2 bleeding (save ends)
        tier2: 17 damage; A < 3 bleeding (save ends)
        tier3: 21 damage; A < 4 bleeding (save ends)
      - name: Effect
        effect: If the target is frightened, this ability gains an edge.
  - type: feature
    feature_type: ability
    name: Tail Spike
    icon: 🏹
    keywords:
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Ranged 10
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        tier1: 6 damage; M < 2 4 poison damage
        tier2: 11 damage; M < 3 4 poison damage, weakened (save ends)
        tier3: 14 damage; M < 4 8 poison damage, weakened (save ends)
      - cost: 1 Malice
        effect: While weakened this way, a target takes 1d6 poison dam- age at the start
          of each of their turns.
  - type: feature
    feature_type: ability
    name: Harrying Claws
    icon: 🗡
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Maneuver
    distance: Melee 1
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        tier1: Slide 1; A < 2 3 damage
        tier2: Slide 2; A < 3 5 damage
        tier3: Slide 4; A < 4 7 damage
  - type: feature
    feature_type: ability
    name: Reflexive Instinct
    icon: ❗️
    cost: 2 Malice
    keywords:
      - Ranged
    usage: Triggered action
    distance: Ranged 10
    target: The triggering creature
    trigger: A creature within distance deals damage to the manticore.
    effects:
      - name: Effect
        effect: The manticore shifts up to 5 squares into the air, then can use Tail
          Spike against the target.
  - type: feature
    feature_type: ability
    name: Trumpeting Howl
    icon: ☠️
    ability_type: Villain Action 1
    keywords:
      - Area
      - Magic
    usage: "-"
    distance: 5 burst
    target: Each creature in the area
    effects:
      - roll: Power Roll + 4
        tier1: Frightened (EoT); if the target has I < 2 they are instead frightened
          (save ends)
        tier2: Frightened (EoT); if the target has I < 3 they are instead frightened
          (save ends)
        tier3: Frightened (EoT); if the target has I < 4 they are instead dazed (save
          ends)
  - type: feature
    feature_type: ability
    name: Cornered Predator
    icon: ☠️
    ability_type: Villain Action 2
    keywords:
      - "-"
    usage: "-"
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The manticore shifts up to their speed, then can use Tail Spike against
          each enemy within distance of that ability.
  - type: feature
    feature_type: ability
    name: Debilitating Poison
    icon: ☠️
    ability_type: Villain Action 3
    keywords:
      - "-"
    usage: "-"
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The manticore sours their poison with enmity. Until the end of the
          encounter, the manticore has a double edge on power rolls against
          weakened creatures. Additionally, any creature weakened by the
          manticore's Tail Spike ability has their speed halved and takes an
          extra 3 poison damage at the start of each of their turns.
~~~