---
agility: 3
ancestry:
- Fey
- Humanoid
- Wode Elf
ev: '20'
file_basename: Wode Elf Warleader
file_dpath: Monsters/Elves Wode/Statblocks
free_strike: 5
intuition: 2
item_id: wode-elf-warleader
item_index: '232'
item_name: Wode Elf Warleader
level: 3
might: 2
presence: 2
reason: 2
roles:
- Leader
scc:
- mcdm.monsters.v1:monster:wode-elf-warleader
scdc:
- 1.1.1:2:232
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 2
stamina: '120'
type: monster
---

~~~ds-statblock
type: statblock
name: Wode Elf Warleader
level: 3
roles:
  - Leader
ancestry:
  - Fey
  - Humanoid
  - Wode Elf
ev: "20"
stamina: "120"
speed: 7
movement: Teleport
size: 1M
stability: 2
free_strike: 5
might: 2
agility: 3
reason: 2
intuition: 2
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Wodeblade
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Magic
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 3
        tier1: 8 damage; M < 1 restrained (save ends)
        tier2: 12 damage; M < 2 restrained (save ends)
        tier3: 15 damage; M < 3 restrained (save ends)
      - name: Effect
        effect: The warleader can teleport up to 3 squares between each strike.
      - cost: 2 Malice
        effect: A target restrained by this ability takes an extra 3 damage.
  - type: feature
    feature_type: ability
    name: Fairness Is a Human Concept
    icon: ❇️
    cost: 5 Malice
    keywords:
      - Area
    usage: Maneuver
    distance: 10 burst
    target: Each ally in the area
    effects:
      - name: Effect
        effect: Each non-minion target can make a free strike, then each target shifts
          up to 3 squares. A target who has cover or concealment at the end of
          this shift can attempt to hide at the end of the warleader's turn.
  - type: feature
    feature_type: ability
    name: Wode Sickness
    icon: ❗️
    keywords:
      - Ranged
    usage: Triggered action
    distance: Ranged 10
    target: One enemy
    trigger: An ally ends their turn.
    effects:
      - name: Effect
        effect: The target must not have taken their turn this round. The target takes
          their turn immediately, and if they have P < 2 they are bleeding and
          take a bane on strikes until the end of their turn.
  - type: feature
    feature_type: trait
    name: End Effect
    icon: ⭐️
    effects:
      - effect: At the end of each of their turns, the warleader can take 5 damage to
          end one effect on them that can be ended by a saving throw. This
          damage can't be reduced in any way.
  - type: feature
    feature_type: trait
    name: Into the Green
    icon: ⭐️
    effects:
      - effect: The warleader can attempt to hide at the end of each of their turns.
  - type: feature
    feature_type: trait
    name: Masking Glamor
    icon: ⭐️
    effects:
      - effect: Abilities targeting the warleader that would take a bane from cover or
          concealment have a double bane instead.
  - type: feature
    feature_type: ability
    name: You Will All Witness my Blade
    icon: ☠️
    ability_type: Villain Action 1
    keywords:
      - Area
    usage: "-"
    distance: 5 burst
    target: Each enemy in the area
    effects:
      - name: Effect
        effect: The warleader uses Wodeblade against each target and gains an edge on
          the power roll.
  - type: feature
    feature_type: ability
    name: Suppressing Volley
    icon: ☠️
    ability_type: Villain Action 2
    keywords:
      - Area
    usage: "-"
    distance: 5 burst
    target: Each ally in the area
    effects:
      - name: Effect
        effect: The warleader can use Wodeblade. Each target can then make a free
          strike.
  - type: feature
    feature_type: ability
    name: Is It Now or Is It Then?
    icon: ☠️
    ability_type: Villain Action 3
    keywords:
      - Area
    usage: "-"
    distance: 5 burst
    target: Self and each ally in the area
    effects:
      - name: Effect
        effect: Each target is invisible until the start of the next round. The
          warleader then uses Wodeblade.
~~~