---
file_basename: Radenwight Malice
file_dpath: Monsters/Radenwights/Features
item_id: radenwight-malice-malice-features
item_index: '17'
item_name: Radenwight Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:radenwight-malice-malice-features
scdc:
- 1.1.1:2.2:17
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
name: Radenwight Malice
type: Malice Features
flavor: At the start of any radenwight's turn, you can spend Malice to activate
  one of the following features.
stats: []
features:
  - name: Trouser Cut
    icon: 🗡
    cost: 3 Malice
    keywords:
      - Magic
      - Melee
    type: Main action
    distance: Melee 1
    target: One creature
    effects:
      - roll: Power Roll + 2
        t1: 7 damage; push 3
        t2: 10 damage; push 3, taunted (EoT)
        t3: 13 damage; push 5, taunted (EoT)
      - effect: If the target is wearing clothing covering the lower half of their body,
          they must use a maneuver once to pull that clothing up before they can
          move.
        name: Effect
      - effect: This ability can't be used by a minion.
        name: Special
  - name: Rat Race
    icon: ⭐️
    cost: 5 Malice
    effects:
      - effect: Each radenwight in the encounter shifts up to their speed. If a
          radenwight ends this shift adjacent to one or more radenwights, they
          can make a melee free strike against each enemy adjacent to them.
  - name: Rally the Rodents
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
        t1: 7 sonic damage; the target can't take a respite activity during their next
          respite
        t2: 5 sonic damage
        t3: No effect.
~~~