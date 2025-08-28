---
agility: 2
ancestry:
- Humanoid
- Rival
ev: '16'
file_basename: Rival Shadow
file_dpath: Monsters/Rivals/1st Echelon/Statblocks
free_strike: 5
intuition: 0
item_id: rival-shadow
item_index: '13'
item_name: Rival Shadow
level: 2
might: 0
presence: 1
reason: 0
roles:
- Elite Ambusher
scc:
- mcdm.monsters.v1:monster:rival-shadow
scdc:
- 1.1.1:2:13
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 1
stamina: '80'
type: monster
---

~~~ds-statblock
name: Rival Shadow
level: 2
roles:
  - Elite Ambusher
ancestry:
  - Humanoid
  - Rival
ev: "16"
stamina: "80"
speed: 7
size: 1M
stability: 1
free_strike: 5
might: 0
agility: 2
reason: 0
intuition: 0
presence: 1
traits:
  - name: Exploit Opening
    effects:
      - effect: The shadow deals an extra 5 damage to any bleeding target.
  - name: Rivalry
    effects:
      - effect: At the start of an encounter, the shadow chooses one creature within
          their line of effect. Both the shadow and the creature can add a d3
          roll to power rolls they make against each other.
abilities:
  - name: Swift Serration
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
      - roll: Power Roll + 2
        t1: 7 damage
        t2: 11 damage
        t3: 14 damage; A < 2 bleeding (save ends)
      - effect: The shadow can teleport up to 5 squares, then can attempt to hide.
        cost: 1 Malice
  - name: Poison the Blade
    icon: 👤
    keywords:
      - "-"
    type: Maneuver
    distance: Self
    target: Self
    effects:
      - effect: The shadow coats their weapon with poison. They gain an edge on their
          next strike, and any potency for that strike increases by 1.
        name: Effect
~~~