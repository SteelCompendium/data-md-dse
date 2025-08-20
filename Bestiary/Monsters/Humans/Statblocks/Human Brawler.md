---
agility: 1
ancestry:
- Human
- Humanoid
ev: '6'
file_basename: Human Brawler
file_dpath: Monsters/Humans/Statblocks
free_strike: 4
intuition: 0
item_id: human-brawler
item_index: '167'
item_name: Human Brawler
level: 1
might: 2
presence: 0
reason: 0
roles:
- Platoon Brute
scc:
- mcdm.monsters.v1:monster:human-brawler
scdc:
- 1.1.1:2:167
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '40'
type: monster
---

```ds-statblock
name: Human Brawler
level: 1
roles:
  - Platoon Brute
ancestry:
  - Human
  - Humanoid
ev: "6"
stamina: "40"
immunities:
  - Corruption 1
  - psychic 1
speed: 5
size: 1M
stability: 0
free_strike: 4
might: 2
agility: 1
reason: 0
intuition: 0
presence: 0
traits:
  - name: Shoot the Hostage
    effects:
      - effect: The brawler halves the damage from any strike if they have a creature or
          object grabbed of size 1S or larger. The grabbed creature or object
          takes the remaining damage.
  - name: Supernatural Insight
    effects:
      - effect: The brawler ignores concealment if it's granted by a supernatural
          effect.
abilities:
  - name: Haymaker
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
        t1: 6 damage
        t2: 9 damage
        t3: 12 damage; M < 2 grabbed and the target takes a bane on the Escape Grab
          maneuver
      - effect: A target who is already grabbed takes an extra 2 damage.
  - name: Throw
    cost: 1 Malice
    keywords:
      - Melee
    type: Maneuver
    distance: Melee 1
    target: One creature grabbed by the brawler
    effects:
      - effect: The brawler pushes the target up to 5 squares.
```