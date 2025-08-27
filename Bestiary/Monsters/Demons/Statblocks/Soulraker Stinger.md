---
agility: -1
ancestry:
- Abyssal
- Demon
- Soulraker
ev: 9 for four minions
file_basename: Soulraker Stinger
file_dpath: Monsters/Demons/Statblocks
free_strike: 4
intuition: 4
item_id: soulraker-stinger
item_index: '261'
item_name: Soulraker Stinger
level: 7
might: 0
presence: 0
reason: 4
roles:
- Minion Artillery
scc:
- mcdm.monsters.v1:monster:soulraker-stinger
scdc:
- 1.1.1:2:261
size: 1M
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '10'
type: monster
---

```ds-statblock
name: Soulraker Stinger
level: 7
roles:
  - Minion Artillery
ancestry:
  - Abyssal
  - Demon
  - Soulraker
ev: 9 for four minions
stamina: "10"
weaknesses:
  - Holy 5
speed: 6
movement: Climb
size: 1M
stability: 0
free_strike: 4
with_captain: Gain an edge on strikes
might: 0
agility: -1
reason: 4
intuition: 4
presence: 0
traits:
  - name: Abyssal Buzzing
    effects:
      - effect: Any enemy who starts their turn with two or more soulraker minions
          adjacent to them takes 3 sonic damage.
abilities:
  - name: Barb Launch
    icon: 🏹
    cost: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Ranged 20
    target: One creature per minion
    effects:
      - roll: Power Roll + 4
        t1: 4 poison damage
        t2: 7 poison damage
        t3: 8 poison damage
      - effect: All soulraker demons have concealment from the target until the start of
          the stinger's next turn.
        name: Effect
```