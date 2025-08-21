---
agility: 2
ancestry:
- Humanoid
- Orc
ev: '10'
file_basename: Orc Bloodrunner
file_dpath: Monsters/Orcs/Statblocks
free_strike: 5
intuition: 1
item_id: orc-bloodrunner
item_index: '126'
item_name: Orc Bloodrunner
level: 3
might: 2
presence: 1
reason: 0
roles:
- Platoon Harrier
scc:
- mcdm.monsters.v1:monster:orc-bloodrunner
scdc:
- 1.1.1:2:126
size: 1M
source: mcdm.monsters.v1
speed: 8
stability: 0
stamina: '50'
type: monster
---

```ds-statblock
name: Orc Bloodrunner
level: 3
roles:
  - Platoon Harrier
ancestry:
  - Humanoid
  - Orc
ev: "10"
stamina: "50"
speed: 8
size: 1M
stability: 0
free_strike: 5
might: 2
agility: 2
reason: 0
intuition: 1
presence: 1
traits:
  - name: Unimpeded
    effects:
      - effect: The bloodrunner can end their movement in a prone creature's space. The
          first time on a turn that a bloodrunner enters any creature's space,
          that creature takes 3 damage.
  - name: Relentless
    effects:
      - effect: If the bloodrunner is reduced to 0 Stamina, they can make a free strike
          before dying. If the target of the free strike is reduced to 0
          Stamina, the bloodrunner is reduced to 1 Stamina instead.
abilities:
  - name: Shield Bash
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 7 damage; push special
        t2: 10 damage; push special
        t3: 13 damage; push special or prone
      - effect: The forced movement distance is equal to the number of squares the
          bloodrunner moved on their turn before using this ability. An ally
          targeted by this ability ignores the damage and can move up to that
          same distance.
        name: Effect
      - effect: An ally targeted by this ability can make a free strike after the forced
          movement is resolved.
        cost: 2 Malice
```