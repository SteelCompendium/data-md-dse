---
agility: 5
ancestry:
- Humanoid
- Rival
ev: '48'
file_basename: Rival Shadow
file_dpath: Monsters/Rivals/4th Echelon/Statblocks
free_strike: 10
intuition: 2
item_id: rival-shadow
item_index: '34'
item_name: Rival Shadow
level: 10
might: 0
presence: 4
reason: 3
roles:
- Elite Ambusher
scc:
- mcdm.monsters.v1:monster:rival-shadow
scdc:
- 1.1.1:2:34
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '240'
type: monster
---

~~~ds-statblock
name: Rival Shadow
level: 10
roles:
  - Elite Ambusher
ancestry:
  - Humanoid
  - Rival
ev: "48"
stamina: "240"
speed: 5
size: 1M
stability: 1
free_strike: 10
might: 0
agility: 5
reason: 3
intuition: 2
presence: 4
traits:
  - name: Exploit Weakness
    effects:
      - effect: The shadow deals an extra 10 damage to any target affected by a
          condition.
  - name: Rivalry
    effects:
      - effect: At the start of an encounter, the shadow chooses one creature within
          their line of effect. Both the shadow and the creature can add a d3
          roll to power rolls they make against each other.
abilities:
  - name: A Hush of Ash
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
      - roll: Power Roll + 5
        t1: 15 damage; A < 3 bleeding (save ends)
        t2: 21 damage; A < 4 bleeding (save ends)
        t3: 25 damage; A < 5 bleeding (save ends)
      - effect: The shadow can teleport up to 10 squares, then can attempt to hide.
        cost: 1 Malice
  - name: Envenomed Steel
    icon: 👤
    keywords:
      - "-"
    type: Maneuver
    distance: Self
    target: Self
    effects:
      - effect: The shadow coats their weapon with poison. They have a double edge on
          their next strike, any potency for that strike increases by 2, and if
          the target has M < 4, they are weakened (save ends).
        name: Effect
~~~