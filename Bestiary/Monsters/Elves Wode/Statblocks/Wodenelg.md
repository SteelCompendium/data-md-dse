---
agility: 1
ancestry:
- Plant
- Wode Elf
ev: '6'
file_basename: Wodenelg
file_dpath: Monsters/Elves Wode/Statblocks
free_strike: 3
intuition: 0
item_id: wodenelg
item_index: '227'
item_name: Wodenelg
level: 1
might: 2
presence: -1
reason: -1
roles:
- Platoon Mount
scc:
- mcdm.monsters.v1:monster:wodenelg
scdc:
- 1.1.1:2:227
size: '2'
source: mcdm.monsters.v1
speed: 10
stability: 1
stamina: '30'
type: monster
---

```ds-statblock
name: Wodenelg
level: 1
roles:
  - Platoon Mount
ancestry:
  - Plant
  - Wode Elf
ev: "6"
stamina: "30"
speed: 10
size: "2"
stability: 1
free_strike: 3
might: 2
agility: 1
reason: -1
intuition: 0
presence: -1
traits:
  - name: Sure-Footed
    effects:
      - effect: The wodenelg ignores difficult terrain and doesn't provoke oppotunity
          attacks by moving.
  - name: Mounted Stability
    effects:
      - effect: The wodenelg's rider has damage immunity 2.
  - name: Shared Glamor
    effects:
      - effect: If the wodenelg's rider has the Masking Glamor trait, the wodenelg also
          has that trait.
abilities:
  - name: Gore
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 5 damage
        t2: 7 damage
        t3: 9 damage
      - effect: The wodenelg's rider can make a free strike at any point during the
          charge.
        name: Effect
  - name: Where I End the Woods Begin
    icon: 👤
    cost: 3 Malice
    keywords:
      - "-"
    type: Maneuver
    distance: Self
    target: Self
    effects:
      - effect: The wodenelg and their rider become invisible until the start of the
          wodenelg's next turn.
        name: Effect
```