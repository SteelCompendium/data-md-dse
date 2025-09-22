---
agility: 4
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '48'
file_basename: Strategos Alkestis
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 10
intuition: 5
item_id: strategos-alkestis
item_index: '359'
item_name: Strategos Alkestis
level: 10
might: 4
presence: 5
reason: 5
roles:
- Leader
scc:
- mcdm.monsters.v1:monster:strategos-alkestis
scdc:
- 1.1.1:2:359
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '260'
type: monster
---

~~~ds-statblock
type: statblock
name: Strategos Alkestis
level: 10
roles:
  - Leader
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "48"
stamina: "260"
speed: 5
size: 1M
stability: 2
free_strike: 10
might: 4
agility: 4
reason: 5
intuition: 5
presence: 5
features:
  - type: feature
    feature_type: ability
    name: Houndgun and Houndblade
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
      - roll: Power Roll + 5
        tier1: 15 damage; M < 4 bleeding (save ends)
        tier2: 21 damage; M < 5 bleeding (save ends)
        tier3: 25 damage; M < 6 bleeding (save ends)
      - name: Effect
        effect: Each target loses 1d3 Recoveries.
      - cost: 2 Malice
        effect: When a target is made bleeding this way, each ally adjacent to them can
          make a free strike against the target.
  - type: feature
    feature_type: ability
    name: Focus Fire
    icon: 🏹
    keywords:
      - Ranged
    usage: Maneuver
    distance: Ranged 15
    target: One creature or object
    effects:
      - name: Effect
        effect: Until the start of Alkestis's next turn, any effect that reduces the
          damage taken by the target has no effect.
  - type: feature
    feature_type: ability
    name: Artillery Enfilade
    icon: ❗️
    cost: 2 Malice
    keywords:
      - Area
      - Ranged
      - Weapon
    usage: Triggered action
    distance: 7 x 3 line within 10
    target: Each creature and object in the area
    trigger: An ally is reduced to 0 Stamina within 10 squares of Alkestis.
    effects:
      - roll: Power Roll + 5
        tier1: 8 damage; A < 4 slowed (save ends)
        tier2: 13 damage; A < 5 slowed (save ends)
        tier3: 16 damage; A < 6 slowed (save ends)
      - name: Effect
        effect: The area is difficult terrain until the start of the next round.
  - type: feature
    feature_type: trait
    name: End Effect
    icon: ⭐️
    effects:
      - effect: At the end of each of her turns, Alkestis can take 20 damage to end one
          effect on her that can be ended by a saving throw. This damage can't
          be reduced in any way.
  - type: feature
    feature_type: trait
    name: Tactical Brilliance
    icon: ⭐️
    effects:
      - effect: At the start of each of Alkestis's turns, the Director gains 2 Malice.
          While Alkestis is alive and in the encounter, the Director also gains
          1 Malice whenever a war dog in the encounter obtains a tier 3 outcome
          on a power roll.
  - type: feature
    feature_type: ability
    name: Fog of War
    icon: ☠️
    ability_type: Villain Action 1
    keywords:
      - "-"
    usage: "-"
    distance: Special
    target: Each ally in the encounter
    effects:
      - name: Effect
        effect: Each target can disappear, then reappear anywhere on the encounter map 3
          or more squares away from any enemy. Additionally, each target has a
          double edge on their next power roll.
  - type: feature
    feature_type: ability
    name: Send in the Second Wave
    icon: ☠️
    ability_type: Villain Action 2
    keywords:
      - Ranged
    usage: "-"
    distance: Ranged 15
    target: Special
    effects:
      - name: Effect
        effect: For each war dog reduced to 0 Stamina in the encounter, a war dog
          shriketrooper appears in an unoccupied space within distance.
  - type: feature
    feature_type: ability
    name: The Silver Wolf's Final Stratagem
    icon: ☠️
    ability_type: Villain Action 3
    keywords:
      - Area
      - Magic
    usage: "-"
    distance: 5 burst
    target: Each creature in the area
    effects:
      - name: Effect
        effect: Until the start of the next round, each target enemy who has I < 4 is
          dazed, each target enemy who has M < 4 is restrained, and each target
          enemy who has A < 4 can't use triggered actions. Additionally, until
          the end of the encounter, Alkestis and each target ally have damage
          immunity 3 and deal an extra 5 damage with strikes.
~~~