---
agility: 2
ancestry:
- Undead
ev: '9'
file_basename: Koptourok
file_dpath: Monsters/Undead/Statblocks
free_strike: 3
intuition: 1
item_id: koptourok
item_index: '59'
item_name: Koptourok
level: 7
might: 4
presence: -1
reason: 0
roles:
- Horde Hexer
scc:
- mcdm.monsters.v1:monster:koptourok
scdc:
- 1.1.1:2:59
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '40'
type: monster
---

```ds-statblock
name: Koptourok
level: 7
roles:
  - Horde Hexer
ancestry:
  - Undead
ev: "9"
stamina: "40"
immunities:
  - Corruption 7
  - poison 7
speed: 5
size: 1M
stability: 1
free_strike: 3
might: 4
agility: 2
reason: 0
intuition: 1
presence: -1
traits:
  - name: Exhale
    effects:
      - effect: The first time the koptourok is made winded by damage that isn't fire
          damage or holy damage, each enemy within 3 squares of them takes 8
          corruption damage. Any enemy who takes this damage and has M < 3 is
          also weakened (save ends)
abilities:
  - name: Choking Grasp
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 5
    target: One creature or object
    effects:
      - roll: Power Roll + 4
        t1: 7 damage; M < 2 grabbed
        t2: 10 damage; M < 3 grabbed
        t3: 11 damage; M < 4 grabbed
      - effect: A creature grabbed this way is suffocating. The koptourok can have up to
          two creatures grabbed at once.
        name: Effect
  - name: Inhale
    cost: 3 Malice
    keywords:
      - Area
      - Magic
    type: Main action
    distance: 5 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 4
        t1: Pull 3; M < 2 5 corruption damage
        t2: Pull 5; M < 3 5 corruption damage
        t3: Pull 7; M < 4 5 corruption damage
      - effect: This ability gains an edge against any target grabbed by the koptourok.
          If one or more targets are pulled adjacent to the kop- tourok, the
          koptourok can fly until the end of the encounter
        name: Effect
```