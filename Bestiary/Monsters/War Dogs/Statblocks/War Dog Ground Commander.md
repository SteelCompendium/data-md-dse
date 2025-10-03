---
agility: 2
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '20'
file_basename: War Dog Ground Commander
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 5
intuition: 2
item_id: war-dog-ground-commander
item_index: '355'
item_name: War Dog Ground Commander
level: 3
might: 3
presence: 2
reason: 3
roles:
- Leader
scc:
- mcdm.monsters.v1:monster:war-dog-ground-commander
scdc:
- 1.1.1:2:355
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '120'
type: monster
---

~~~ds-statblock
type: statblock
name: War Dog Ground Commander
level: 3
roles:
  - Leader
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "20"
stamina: "120"
speed: 5
size: 1M
stability: 2
free_strike: 5
might: 3
agility: 2
reason: 3
intuition: 2
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Conditioning Spear
    icon: ⚔️
    ability_type: Signature Ability
    keywords:
      - Melee
      - Psionic
      - Ranged
      - Strike
    usage: Main action
    distance: Melee 1 or ranged 5
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 3
        tier1: 8 damage; pull 1
        tier2: 12 damage; pull 2
        tier3: 15 damage; pull 3
      - name: Effect
        effect: One ally within 10 squares of the ground commander can make a free
          strike.
      - cost: 1 Malice
        effect: A target who has I < 2 and who is adjacent to the ground commander after
          this ability is resolved is grabbed (save ends). This grab can't be
          escaped using the Escape Grab maneuver. The ground commander can grab
          up to two creatures at a time.
  - type: feature
    feature_type: ability
    name: Highest Posthumous Promotion
    icon: ❇️
    keywords:
      - Area
      - Magic
    usage: Maneuver
    distance: 10 burst
    target: Each war dog in the area
    effects:
      - name: Effect
        effect: Any target who has a loyalty collar is reduced to 0 Stamina.
  - type: feature
    feature_type: ability
    name: Final Orders
    icon: ❗️
    keywords:
      - Magic
      - Ranged
    usage: Triggered action
    distance: Ranged 10
    target: One ally
    trigger: The target takes damage, is force moved, or is reduced to 0 Stamina.
    effects:
      - name: Effect
        effect: Even if reduced to 0 Stamina, the target moves up to their speed and can
          make a free strike after the triggering effect is resolved. The target
          then immediately dies.
  - type: feature
    feature_type: trait
    name: End Effect
    icon: ⭐️
    effects:
      - effect: At the end of each of their turns, the ground commander can take 5
          damage to end one effect on them that can be ended by a saving throw.
          This damage can't be reduced in any way.
  - type: feature
    feature_type: trait
    name: Loyalty Collar
    icon: ⭐️
    effects:
      - effect: When the ground commander is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 2d6 damage to each adjacent enemy and object.
  - type: feature
    feature_type: ability
    name: Combined Arms
    icon: ☠️
    ability_type: Villain Action 1
    keywords:
      - Area
    usage: "-"
    distance: 10 burst
    target: Each ally in the area
    effects:
      - name: Effect
        effect: Each target can make a ranged free strike, then immediately use the
          Charge main action.
  - type: feature
    feature_type: ability
    name: Make an Example of Them
    icon: ☠️
    ability_type: Villain Action 2
    keywords:
      - Magic
      - Ranged
    usage: "-"
    distance: Ranged 10
    target: One enemy
    effects:
      - name: Effect
        effect: Each ally within 5 squares of the target moves up to their speed and can
          make a free strike against the target. If the target has I < 2, they
          are frightened of the ground commander (save ends).
  - type: feature
    feature_type: ability
    name: Claim Them for the Body Banks
    icon: ☠️
    ability_type: Villain Action 3
    keywords:
      - Area
      - Magic
    usage: "-"
    distance: 10 burst
    target: Each creature in the area
    effects:
      - name: Effect
        effect: Each target ally shifts up to 2 squares and can use the Grab maneuver.
          Until the end of the encounter, each target enemy takes a bane on the
          Escape Grab maneuver.
~~~