---
agility: 1
ancestry:
- Eyestalk
- Horror
- Overmind
ev: '-'
file_basename: Compulsion Eye
file_dpath: Monsters/Xorannox the Tyract/Statblocks
free_strike: 3
intuition: 1
item_id: compulsion-eye
item_index: '318'
item_name: Compulsion Eye
level: 6
might: -1
presence: -1
reason: 4
roles:
- Controller
scc:
- mcdm.monsters.v1:monster:compulsion-eye
scdc:
- 1.1.1:2:318
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '30'
type: monster
---

~~~ds-statblock
name: Compulsion Eye
level: 6
roles:
  - Controller
ancestry:
  - Eyestalk
  - Horror
  - Overmind
ev: "-"
stamina: "30"
speed: 5
movement: Fly, hover
size: 1M
stability: 0
free_strike: 3
might: -1
agility: 1
reason: 4
intuition: 1
presence: -1
traits:
  - name: Psionic Barrier
    effects:
      - effect: The compulsion eye has damage immunity 15. When they use a main action,
          they lose this immunity until the end of the round.
abilities:
  - name: Compulsion Beam
    icon: 🏹
    cost: Signature Ability
    keywords:
      - Psionic
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 6
    target: One creature
    effects:
      - roll: Power Roll + 4
        t1: I < 2 the target is charmed
        t2: I < 3 the target is charmed
        t3: I < 4 the target is charmed
      - effect: As a free triggered action, a charmed target immediately moves up to
          their speed and can make a free strike against an enemy of Xorannox's
          choice. The target is then no longer charmed.
        name: Effect
~~~