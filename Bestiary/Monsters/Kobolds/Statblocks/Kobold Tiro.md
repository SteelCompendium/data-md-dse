---
agility: 2
ancestry:
- Humanoid
- Kobold
ev: 3 for four minions
file_basename: Kobold Tiro
file_dpath: Monsters/Kobolds/Statblocks
free_strike: 1
intuition: 0
item_id: kobold-tiro
item_index: '96'
item_name: Kobold Tiro
level: 1
might: 0
presence: 0
reason: 0
roles:
- Minion Defender
scc:
- mcdm.monsters.v1:monster:kobold-tiro
scdc:
- 1.1.1:2:96
size: 1S
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '5'
type: monster
---

~~~ds-statblock
name: Kobold Tiro
level: 1
roles:
  - Minion Defender
ancestry:
  - Humanoid
  - Kobold
ev: 3 for four minions
stamina: "5"
speed: 5
size: 1S
stability: 0
free_strike: 1
with_captain: +1 bonus to speed
might: 0
agility: 2
reason: 0
intuition: 0
presence: 0
traits:
  - name: Shield? Shield!
    effects:
      - effect: While adjacent to an ally who also has this trait, the tiro has
          stability 1, has cover, and grants cover to allies.
abilities:
  - name: Pugio
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        t1: 1 damage
        t2: 2 damage; the tiro can shift 1 square
        t3: 3 damage; the tiro shifts up to 2 squares
      - effect: The target can't shift until the start of the tiro's next turn
        name: Effect
~~~