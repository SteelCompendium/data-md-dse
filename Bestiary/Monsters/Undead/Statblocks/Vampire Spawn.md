---
agility: 3
ancestry:
- Undead
- Vampire
ev: '6'
file_basename: Vampire Spawn
file_dpath: Monsters/Undead/Statblocks
free_strike: 2
intuition: 1
item_id: vampire-spawn
item_index: '54'
item_name: Vampire Spawn
level: 4
might: 2
presence: 2
reason: -1
roles:
- Horde Harrier
scc:
- mcdm.monsters.v1:monster:vampire-spawn
scdc:
- 1.1.1:2:54
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '30'
type: monster
---

```ds-statblock
name: Vampire Spawn
level: 4
roles:
  - Horde Harrier
ancestry:
  - Undead
  - Vampire
ev: "6"
stamina: "30"
immunities:
  - Corruption 4
  - poison 4
speed: 5
movement: Climb
size: 1M
stability: 0
free_strike: 2
might: 2
agility: 3
reason: -1
intuition: 1
presence: 2
traits:
  - name: Unslakable Bloodthirst
    effects:
      - effect: The vampire spawn has speed 10 while any creature within 10 squares of
          them is bleeding. The vampire spawn must use Exsanguinating Bite
          against a bleeding creature on their turn if they are able to.
abilities:
  - name: Exsanguinating Bite
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 3
        t1: 5 damage
        t2: 7 corruption damage; M < 2 bleeding (save ends)
        t3: 9 corruption damage; M < 3 bleeding (save ends)
      - effect: The vampire spawn regains Stamina equal to any corruption damage dealt.
        name: Effect
      - effect: The target takes an additional 3 corruption damage.
        cost: 1 Malice
  - name: Vampiric Celerity
    icon: 👤
    keywords:
      - "-"
    type: Maneuver
    distance: Self
    target: Self
    effects:
      - effect: The vampire spawn can shift 1 square, then move up to their speed. The
          next ability the vampire uses before the start of their next turn
          gains an edge.
        name: Effect
```