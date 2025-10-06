---
file_basename: Radenwight Malice
file_dpath: Monsters/Radenwights/Features
item_id: radenwight-malice-malice-features
item_index: '20'
item_name: Radenwight Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:radenwight-malice-malice-features
scdc:
- 1.1.1:2.2:20
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
type: featureblock
featureblock_type: Malice Features
name: Radenwight Malice
flavor: At the start of any radenwight's turn, you can spend Malice to activate
  one of the following features.
features:
  - type: feature
    feature_type: ability
    name: Trouser Cut
    icon: 🗡
    cost: 3 Malice
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature
    effects:
      - roll: Power Roll + 2
        tier1: 7 damage; push 3
        tier2: 10 damage; push 3, taunted (EoT)
        tier3: 13 damage; push 5, taunted (EoT)
      - name: Effect
        effect: If the target is wearing clothing covering the lower half of their body,
          they must use a maneuver once to pull that clothing up before they can
          move.
      - name: Special
        effect: This ability can't be used by a minion.
  - type: feature
    feature_type: trait
    name: Rat Race
    icon: ⭐️
    cost: 5 Malice
    effects:
      - effect: Each radenwight in the encounter shifts up to their speed. If a
          radenwight ends this shift adjacent to one or more radenwights, they
          can make a melee free strike against each enemy adjacent to them.
  - type: feature
    feature_type: trait
    name: Rally the Rodents
    icon: 🔳
    cost: 7 Malice
    effects:
      - effect: >-
          A radenwight uses music to coordinate living rats, forming a 10 wall
          of rats scurrying atop one another into unoccupied spaces anywhere on
          the encounter map. The wall doesn't block line of effect for
          radenwights and their allies, but it does for other creatures as the
          rats coordinate their movements with the radenwights. Each square of
          the wall has 10 Stamina.


          If the last radenwight in the encounter dies and the wall is still
          standing, the rats let out a hideous screech as they disperse. Each
          enemy on the encounter map makes an Intuition test.
        tier1: 7 sonic damage; the target can't take a respite activity during their
          next respite
        tier2: 5 sonic damage
        tier3: No effect.
~~~