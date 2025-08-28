---
agility: 4
ancestry:
- Humanoid
- Rival
ev: '40'
file_basename: Rival Shadow
file_dpath: Monsters/Rivals/3rd Echelon/Statblocks
free_strike: 9
intuition: 0
item_id: rival-shadow
item_index: '27'
item_name: Rival Shadow
level: 8
might: 0
presence: 3
reason: 2
roles:
- Elite Ambusher
scc:
- mcdm.monsters.v1:monster:rival-shadow
scdc:
- 1.1.1:2:27
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 1
stamina: '200'
type: monster
---

```ds-statblock
name: Rival Shadow
level: 8
roles:
  - Elite Ambusher
ancestry:
  - Humanoid
  - Rival
ev: "40"
stamina: "200"
speed: 7
size: 1M
stability: 1
free_strike: 9
might: 0
agility: 4
reason: 2
intuition: 0
presence: 3
traits:
  - name: Exploit Weakness
    effects:
      - effect: The shadow deals an extra 9 damage to any target affected by a
          condition.
  - name: Rivalry
    effects:
      - effect: At the start of an encounter, the shadow chooses one creature within
          their line of effect. Both the shadow and the creature can add a d3
          roll to power rolls they make against each other.
abilities:
  - name: Assail and Serrate
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        t1: 13 damage; A < 2 bleeding (save ends)
        t2: 18 damage; A < 3 bleeding (save ends)
        t3: 22 damage; A < 4 bleeding and weakened (save ends)
      - effect: The shadow can teleport up to 7 squares, then can attempt to hide.
        cost: 1 Malice
  - name: Poison the Blade
    icon: 👤
    keywords:
      - "-"
    type: Maneuver
    distance: Self
    target: Self
    effects:
      - effect: The shadow coats their weapon with poison. They have a double edge on
          their next strike, and any potency for that strike increases by 2.
        name: Effect
```