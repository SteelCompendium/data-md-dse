---
agility: 5
ancestry:
- Undead
- Vampire
ev: '144'
file_basename: Count Rhodar von Glauer
file_dpath: Monsters/Count Rhodar Von Glauer/Statblocks
free_strike: 10
intuition: 2
item_id: count-rhodar-von-glauer
item_index: '287'
item_name: Count Rhodar von Glauer
level: 10
might: 3
presence: 3
reason: 2
roles:
- Solo
scc:
- mcdm.monsters.v1:monster:count-rhodar-von-glauer
scdc:
- 1.1.1:2:287
size: 1M
source: mcdm.monsters.v1
speed: 12
stability: 3
stamina: '650'
type: monster
---

~~~ds-statblock
type: statblock
name: Count Rhodar von Glauer
level: 10
roles:
  - Solo
ancestry:
  - Undead
  - Vampire
ev: "144"
stamina: "650"
immunities:
  - Corruption 10
  - poison 10
speed: 12
movement: Fly, hover, teleport
size: 1M
stability: 3
free_strike: 10
might: 3
agility: 5
reason: 2
intuition: 2
presence: 3
features:
  - type: feature
    feature_type: trait
    name: Solo Monster
    icon: ☠️
    effects:
      - name: End Effect
        effect: At the end of each of his turns, Rhodar can take 20 dam- age to end one
          effect on him that can be ended by a saving throw. This damage can't
          be reduced in any way.
      - name: Solo Turns
        effect: Rhodar can take two turns each round. He can't take turns consecutively.
  - type: feature
    feature_type: trait
    name: Grave Ward
    icon: ⭐️
    effects:
      - effect: Rhodar has damage immunity 5. If he takes holy damage, he loses this
          immunity until the end of the round.
  - type: feature
    feature_type: trait
    name: Thin the Blood
    icon: ⭐️
    effects:
      - effect: Each enemy within 10 squares of Rhodar takes a -2 penalty to saving
          throws.
  - type: feature
    feature_type: ability
    name: Spear of the Damned
    icon: ⚔️
    ability_type: Signature Ability
    keywords:
      - Magic
      - Melee
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 2 or ranged 15
    target: Three creatures or objects
    effects:
      - roll: Power Roll + 5
        tier1: 13 damage; A < 4 restrained (save ends)
        tier2: 18 damage; A < 5 restrained (save ends)
        tier3: 21 damage; A < 6 restrained (save ends)
      - name: Effect
        effect: A target restrained this way is impaled by a spear. Rhodar has four
          spears, each of which can be used to impale a target. At the start of
          each of his turns, Rhodar can summon any of his spears back to
          himself, ending the restrained condition on an impaled target.
  - type: feature
    feature_type: ability
    name: Disarming Glare
    icon: ❇️
    keywords:
      - Area
      - Magic
    usage: Main action
    distance: 5 burst
    target: Each enemy in the area
    effects:
      - name: Effect
        effect: Each target makes an Intuition test.
        tier1: 16 corruption damage; frightened (save ends)
        tier2: 13 corruption damage; frightened (EoT)
        tier3: 8 corruption damage
      - effect: While a target is frightened this way, Rhodar ignores banes and double
          banes on abilities used against them.
  - type: feature
    feature_type: ability
    name: Vermilion Fangs
    icon: 🗡
    cost: 3 Malice
    keywords:
      - Melee
      - Weapon
      - Strike
    usage: Main action
    distance: Melee 1
    target: One creature
    effects:
      - roll: Power Roll + 5
        tier1: 17 corruption damage; M < 4 bleeding (save ends) and prone
        tier2: 24 corruption damage; prone; M < 5 bleeding (save ends)
        tier3: 30 corruption damage; prone; M < 6 the target is bleeding until the end
          of the encounter
      - name: Effect
        effect: Rhodar regains Stamina equal to half the damage dealt.
  - type: feature
    feature_type: ability
    name: Sanguineous Flourish
    icon: ❇️
    cost: 5 Malice
    keywords:
      - Area
      - Weapon
    usage: Main action
    distance: 2 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 5
        tier1: 6 damage, 2 corruption damage; push 2; M < 4 bleeding (save ends)
        tier2: 6 damage, 7 corruption damage; push 5; M < 5 bleeding (save ends)
        tier3: 6 damage, 10 corruption damage; push 7; M < 6 bleeding (save ends)
      - name: Effect
        effect: Rhodar shifts up to his speed before or after using this ability He
          regains Stamina equal to half the total corruption damage dealt.
  - type: feature
    feature_type: ability
    name: Vengeance of Rhöl
    icon: 🔳
    cost: 2 Malice
    keywords:
      - Area
      - Magic
      - Ranged
    usage: Maneuver
    distance: Two 3 cubes within 5
    target: Special
    effects:
      - name: Effect
        effect: Each area is saturated with vengeful spirits until the end of the round.
          Any enemy who enters the area for the first time in a round or starts
          their turn there takes 5 corruption damage. At the end of the round,
          the spirits violently disperse. Each enemy within 2 squares of an area
          and has P < 5 is weakened (save ends).
  - type: feature
    feature_type: ability
    name: Reactive Rebuke
    icon: ❗️
    cost: 2 Malice
    keywords:
      - Magic
      - Ranged
    usage: Triggered action
    distance: Ranged 10
    target: The triggering creature
    trigger: A creature within distance makes a strike against Rhodar.
    effects:
      - name: Effect
        effect: A target who has I < 5 is frightened. This effect ends if the target is
          11 or more squares from Rhodar.
  - type: feature
    feature_type: trait
    name: Lord's Bloodthirst
    icon: ⭐️
    effects:
      - effect: Rhodar has speed 15 and an edge on power rolls while any creature within
          20 squares of him is bleeding. Any bleeding creature within 10 squares
          of Rhodar can't hide.
  - type: feature
    feature_type: ability
    name: Red Tide
    icon: ☠️
    ability_type: Villain Action 1
    keywords:
      - Area
      - Magic
      - Ranged
    usage: "-"
    distance: 8 cube within 15
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 5
        tier1: 8 corruption damage; A < 4 the target is blood soaked (save ends)
        tier2: 13 corruption damage; A < 5 the target is blood soaked (save ends)
        tier3: 16 corruption damage; A < 6 the target is blood soaked until the end of
          the encounter
      - name: Effect
        effect: While a creature is blood soaked, Rhodar has a double edge on abilities
          used against them.
  - type: feature
    feature_type: ability
    name: Sanguine Mist
    icon: ☠️
    ability_type: Villain Action 2
    keywords:
      - Area
      - Magic
    usage: "-"
    distance: 5 burst
    target: Each enemy in the area
    effects:
      - name: Effect
        effect: Each target makes a Presence test.
        tier1: 16 corruption damage; the target is bleeding until the end of the
          encounter
        tier2: 13 corruption damage; bleeding (save ends)
        tier3: 8 corruption damage
      - name: Effect
        effect: Rhodar teleports to an unoccupied space in the area. If he has lost the
          damage immunity from his Grave Ward trait, he regains it.
  - type: feature
    feature_type: ability
    name: Fires of Dracul
    icon: ☠️
    ability_type: Villain Action 3
    keywords:
      - Area
      - Magic
    usage: "-"
    distance: 15 x 3 line within 1
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 5
        tier1: 10 fire damage; R < 4 weakened (save ends)
        tier2: 16 fire damage; R < 5 weakened (save ends)
        tier3: 20 fire damage; R < 6 weakened (save ends)
      - name: Effect
        effect: Rhodar teleports to an unoccupied space adjacent to one target after the
          ability resolve.
~~~