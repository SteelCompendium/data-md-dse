---
agility: 2
ancestry:
- Undead
ev: '6'
file_basename: Wraith
file_dpath: Monsters/Undead/Statblocks
free_strike: 2
intuition: 1
item_id: wraith
item_index: '73'
item_name: Wraith
level: 4
might: -2
presence: 3
reason: 1
roles:
- Horde Hexer
scc:
- mcdm.monsters.v1:monster:wraith
scdc:
- 1.1.1:2:73
size: 1M
source: mcdm.monsters.v1
speed: 8
stability: 1
stamina: '25'
type: monster
---

~~~ds-statblock
type: statblock
name: Wraith
level: 4
roles:
  - Horde Hexer
ancestry:
  - Undead
ev: "6"
stamina: "25"
immunities:
  - Corruption 4
  - poison 4
speed: 8
movement: Fly, hover
size: 1M
stability: 1
free_strike: 2
might: -2
agility: 2
reason: 1
intuition: 1
presence: 3
features:
  - type: feature
    feature_type: ability
    name: Chilling Gravetouch
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Magic
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 3
        tier1: 5 cold damage; P < 1 slowed (save ends)
        tier2: 7 cold damage; P < 2 slowed (save ends)
        tier3: 9 cold damage; P < 3 slowed (save ends)
      - name: Effect
        effect: Any living creature who dies from this damage rises at the start of the
          next round as a ghoul craver under the Director's control.
  - type: feature
    feature_type: ability
    name: Hidden Movement
    icon: 👤
    keywords:
      - "-"
    usage: Maneuver
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The wraith turns invisible, moves up to their speed, and is visible
          again.
  - type: feature
    feature_type: ability
    name: Stolen Vitality
    icon: ❗️
    cost: 1 Malice
    keywords:
      - Magic
      - Ranged
    usage: Free triggered action
    distance: Ranged 5
    target: The triggering creature
    trigger: An enemy within distance regains Stamina.
    effects:
      - name: Effect
        effect: The target regains only half the Stamina, and the wraith regains the
          remaining Stamina.
  - type: feature
    feature_type: trait
    name: Agonizing Phasing
    icon: ⭐️
    effects:
      - effect: The wraith can move through creatures and objects at their usual speed,
          but can't end their turn inside a creature or object. The first time
          in a round that the wraith moves through a creature, that creature
          takes 5 corruption damage and takes a bane on their next strike. The
          wraith doesn't take damage from being force moved into objects.
~~~