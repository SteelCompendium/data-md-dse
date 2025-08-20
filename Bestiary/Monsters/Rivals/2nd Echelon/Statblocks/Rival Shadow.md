---
agility: 3
ancestry:
- Humanoid
- Rival
ev: '28'
file_basename: Rival Shadow
file_dpath: Monsters/Rivals/2nd Echelon/Statblocks
free_strike: 7
intuition: 0
item_id: rival-shadow
item_index: '20'
item_name: Rival Shadow
level: 5
might: 0
presence: 2
reason: 1
roles:
- Elite Ambusher
scc:
- mcdm.monsters.v1:monster:rival-shadow
scdc:
- 1.1.1:2:20
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 1
stamina: '140'
type: monster
---

```ds-statblock
name: Rival Shadow
level: 5
roles:
  - Elite Ambusher
ancestry:
  - Humanoid
  - Rival
ev: "28"
stamina: "140"
speed: 7
size: 1M
stability: 1
free_strike: 7
might: 0
agility: 3
reason: 1
intuition: 0
presence: 2
traits:
  - name: Exploit Opening
    effects:
      - effect: The shadow deals an extra 7 damage to any bleeding target.
  - name: Rivalry
    effects:
      - effect: At the start of an encounter, the shadow chooses one creature within
          their line of effect. Both the shadow and the creature can add a d3
          roll to power rolls they make against each other.
abilities:
  - name: Ambuscade
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 3
        t1: 10 damage
        t2: 15 damage; A < 2 bleeding (save ends)
        t3: 18 damage; A < 3 bleeding (save ends)
      - effect: The shadow can teleport up to 6 squares, then can attempt to hide.
        cost: 1 Malice
  - name: Poison the Blade
    keywords:
      - "-"
    type: Maneuver
    distance: Self
    target: Self
    effects:
      - effect: The shadow coats their weapon with poison. They gain an edge on their
          next strike, and any potency for that strike increases by 1.
```