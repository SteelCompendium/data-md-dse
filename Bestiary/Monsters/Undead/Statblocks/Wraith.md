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

```ds-statblock
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
traits:
  - name: Agonizing Phasing
    effects:
      - effect: The wraith can move through creatures and objects at their usual speed,
          but can't end their turn inside a creature or object. The first time
          in a round that the wraith moves through a creature, that creature
          takes 5 corruption damage and takes a bane on their next strike. The
          wraith doesn't take damage from being force moved into objects
abilities:
  - name: Chilling Gravetouch
    cost: Signature Ability
    keywords:
      - Magic
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 3
        t1: 5 cold damage; P < 1 slowed (save ends)
        t2: 7 cold damage; P < 2 slowed (save ends)
        t3: 9 cold damage; P < 3 slowed (save ends)
      - effect: Any living creature who dies from this damage rises at the start of the
          next round as a ghoul craver under the Director's control.
  - name: Hidden Movement
    keywords:
      - "-"
    type: Maneuver
    distance: Self
    target: Self
    effects:
      - effect: The wraith turns invisible, moves up to their speed, and is visible
          again.
  - name: Stolen Vitality
    cost: 1 Malice
    keywords:
      - Magic
      - Ranged
    type: Free triggered action
    distance: Ranged 5
    target: The triggering creature
    trigger: An enemy within distance regains Stamina.
    effects:
      - effect: The target regains only half the Stamina, and the wraith regains the
          remaining Stamina.
```