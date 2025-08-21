---
agility: 2
ancestry:
- Humanoid
- Soulless
- War Dog
ev: 9 for four minions
file_basename: War Dog Saboteur
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 4
intuition: 3
item_id: war-dog-saboteur
item_index: '375'
item_name: War Dog Saboteur
level: 7
might: -1
presence: 1
reason: 4
roles:
- Minion Ambusher
scc:
- mcdm.monsters.v1:monster:war-dog-saboteur
scdc:
- 1.1.1:2:375
size: 1S
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '12'
type: monster
---

```ds-statblock
name: War Dog Saboteur
level: 7
roles:
  - Minion Ambusher
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: 9 for four minions
stamina: "12"
speed: 6
size: 1S
stability: 0
free_strike: 4
with_captain: +5 bonus to ranged distance
might: -1
agility: 2
reason: 4
intuition: 3
presence: 1
traits:
  - name: Loyalty Collar
    effects:
      - effect: When the saboteur is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 2d6 damage to each adjacent enemy and object.
abilities:
  - name: Fuse-Iron Bomb
    cost: Signature Ability
    keywords:
      - Ranged
      - Weapon
    type: Main action
    distance: Ranged 5
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 4
        t1: 4 fire damage
        t2: 7 fire damage; push
        t3: 8 fire damage; push
      - effect: The space the target occupies fills with dark smoke and blocks line of
          effect until the start of the saboteur's next turn
        name: Effect
```