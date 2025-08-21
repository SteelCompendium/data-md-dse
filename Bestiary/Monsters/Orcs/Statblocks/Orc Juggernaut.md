---
agility: 2
ancestry:
- Humanoid
- Orc
ev: '10'
file_basename: Orc Juggernaut
file_dpath: Monsters/Orcs/Statblocks
free_strike: 5
intuition: -1
item_id: orc-juggernaut
item_index: '137'
item_name: Orc Juggernaut
level: 3
might: 2
presence: 2
reason: -1
roles:
- Platoon Brute
scc:
- mcdm.monsters.v1:monster:orc-juggernaut
scdc:
- 1.1.1:2:137
size: 1L
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '60'
type: monster
---

```ds-statblock
name: Orc Juggernaut
level: 3
roles:
  - Platoon Brute
ancestry:
  - Humanoid
  - Orc
ev: "10"
stamina: "60"
speed: 6
size: 1L
stability: 0
free_strike: 5
might: 2
agility: 2
reason: -1
intuition: -1
presence: 2
traits:
  - name: Blood in the Water
    effects:
      - effect: Whenever the juggernaut willingly moves, they can move 3 additional
          squares if they end their movement closer to a prone creature.
  - name: Relentless
    effects:
      - effect: If the juggernaut is reduced to 0 Stamina, they can make a free strike
          before dying. If the target of the free strike is reduced to 0
          Stamina, the juggernaut is reduced to 1 Stamina instead.
abilities:
  - name: Haymaker Greataxe
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
        t1: 7 damage
        t2: 11 damage; prone
        t3: 14 damage; prone; M < 2 bleeding (save ends)
      - effect: A target who is already prone takes an extra 6 damage.
        name: Effect
  - name: Hrraaaaaagh!
    cost: 1 Malice
    keywords:
      - "-"
    type: Free triggered action
    distance: Self
    target: Self
    trigger: The juggernaut takes damage.
    effects:
      - effect: The juggernaut moves up to their speed and can make a free strike.
        name: Effect
```