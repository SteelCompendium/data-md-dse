---
agility: 1
ancestry:
- Goblin
- Hobgoblin
- Humanoid
- Infernal
ev: '12'
file_basename: Hobgoblin Burning Witch
file_dpath: Monsters/Hobgoblins/Statblocks
free_strike: 5
intuition: 2
item_id: hobgoblin-burning-witch
item_index: '178'
item_name: Hobgoblin Burning Witch
level: 4
might: 0
presence: 3
reason: 2
roles:
- Platoon Controller
scc:
- mcdm.monsters.v1:monster:hobgoblin-burning-witch
scdc:
- 1.1.1:2:178
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '50'
type: monster
---

~~~ds-statblock
name: Hobgoblin Burning Witch
level: 4
roles:
  - Platoon Controller
ancestry:
  - Goblin
  - Hobgoblin
  - Humanoid
  - Infernal
ev: "12"
stamina: "50"
immunities:
  - Fire 4
speed: 5
movement: Teleport
size: 1M
stability: 0
free_strike: 5
might: 0
agility: 1
reason: 2
intuition: 2
presence: 3
traits:
  - name: Infernal Ichor
    effects:
      - effect: When the burning witch is reduced to 0 Stamina, they spray burning
          blood. Each creature adjacent to the burning witch takes 3 fire
          damage.
abilities:
  - name: Soul Burn
    icon: 🏹
    cost: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 10
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 3
        t1: 4 corruption or fire damage
        t2: 6 corruption or fire damage
        t3: 8 corruption or fire damage
      - effect: Each target who has P < 2 is weakened (save ends). Any enemy who starts
          their turn within 3 squares of a target weakened this way and who has
          P < 2 is weakened (save ends).
        cost: 2 Malice
  - name: Burning Legion
    icon: 🏹
    cost: 1 Malice
    keywords:
      - Magic
      - Ranged
    type: Maneuver
    distance: Ranged 10
    target: Three creatures
    effects:
      - effect: Each target can teleport up to 5 squares. Each creature adjacent to a
          target at their destination takes 3 fire damage.
        name: Effect
~~~