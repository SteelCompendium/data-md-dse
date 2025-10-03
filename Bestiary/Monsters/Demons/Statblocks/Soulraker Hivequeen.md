---
agility: -1
ancestry:
- Abyssal
- Demon
- Soulraker
ev: '44'
file_basename: Soulraker Hivequeen
file_dpath: Monsters/Demons/Statblocks
free_strike: 9
intuition: 3
item_id: soulraker-hivequeen
item_index: '275'
item_name: Soulraker Hivequeen
level: 9
might: 5
presence: 2
reason: 3
roles:
- Leader
scc:
- mcdm.monsters.v1:monster:soulraker-hivequeen
scdc:
- 1.1.1:2:275
size: '5'
source: mcdm.monsters.v1
speed: 6
stability: 2
stamina: '240'
type: monster
---

~~~ds-statblock
type: statblock
name: Soulraker Hivequeen
level: 9
roles:
  - Leader
ancestry:
  - Abyssal
  - Demon
  - Soulraker
ev: "44"
stamina: "240"
weaknesses:
  - Holy 5
speed: 6
movement: Fly
size: "5"
stability: 2
free_strike: 9
might: 5
agility: -1
reason: 3
intuition: 3
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Stinging Ovipositor
    icon: ⚔️
    ability_type: Signature Ability
    keywords:
      - Magic
      - Melee
      - Ranged
      - Strike
    usage: Main action
    distance: Melee 1 or ranged 10
    target: Two creatures
    effects:
      - roll: Power Roll + 5
        tier1: 14 poison damage; M < 3 bleeding (save ends)
        tier2: 19 poison damage; M < 4 bleeding (save ends)
        tier3: 23 poison damage; M < 5 the target is implanted
      - name: Effect
        effect: An implanted target has a soulraker handmaiden parasite gestating in
          them (see the handmaiden's Implanted Parasite trait).
  - type: feature
    feature_type: ability
    name: Forced Gestation
    icon: ❇️
    cost: 3 Malice
    keywords:
      - Area
    usage: Maneuver
    distance: 10 burst
    target: Each implanted handmaiden parasite in the area
    effects:
      - name: Effect
        effect: The hivequeen lets loose a subsonic call to each target, forcing them to
          immediately emerge from their host's body as a mature soulraker
          handmaiden and make a free strike.
  - type: feature
    feature_type: ability
    name: For the Queen!
    icon: ❗️
    cost: 2 Malice
    keywords:
      - Area
    usage: Triggered action
    distance: 5 burst
    target: Special
    trigger: The hivequeen is targeted by a strike for the second time on an
      attacker's turn, whether by the attacker or another creature acting on the
      attacker's turn.
    effects:
      - name: Effect
        effect: Two soulraker minions appear within distance.
      - cost: 2 Malice
        effect: A soulraker praetorian also appears within distance.
  - type: feature
    feature_type: trait
    name: Cannibal Queen
    icon: ⭐️
    effects:
      - effect: At the end of their turn, the hivequeen can consume an adjacent
          soulraker demon to end one effect on them that can be ended by a
          saving throw (no action required).
  - type: feature
    feature_type: trait
    name: Hive Soulsight
    icon: ⭐️
    effects:
      - effect: Any creature within 2 squares of a soulraker demon within 100 miles of
          the hivequeen can't be hidden from the hivequeen. The hivequeen has
          line of effect to such creatures.
  - type: feature
    feature_type: ability
    name: Kicking the Nest
    icon: ☠️
    ability_type: Villain Action 1
    keywords:
      - Area
    usage: "-"
    distance: 10 burst
    target: Each soulraker minion in the area
    effects:
      - name: Effect
        effect: Each target can move their speed and make a free strike. If no minions
          are present, four soulraker minions are summoned into unoccupied
          spaces within distance before the hivequeen uses this villain action.
  - type: feature
    feature_type: ability
    name: Buzz Off!
    icon: ☠️
    ability_type: Villain Action 2
    keywords:
      - Area
    usage: "-"
    distance: 5 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 5
        tier1: Push 3; I < 3 dazed (save ends)
        tier2: Push 3; I < 4 dazed (save ends)
        tier3: 11 sonic damage; push 3; I < 5 dazed (save ends)
      - name: Effect
        effect: The hivequeen shifts up to her speed.
  - type: feature
    feature_type: ability
    name: Bomber Wasp Warfare
    icon: ☠️
    ability_type: Villain Action 3
    keywords:
      - Area
      - Magic
      - Ranged
    usage: "-"
    distance: Four 2 cubes within 10
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 4
        tier1: 7 poison damage; M < 3 bleeding (save ends)
        tier2: 11 poison damage; M < 4 bleeding (save ends)
        tier3: 14 poison damage; M < 5 bleeding (save ends)
~~~