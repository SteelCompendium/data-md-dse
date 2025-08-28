---
agility: 2
ancestry:
- Fey
- Humanoid
- Wode Elf
ev: 3 for four minions
file_basename: Wode Elf Runner
file_dpath: Monsters/Elves Wode/Statblocks
free_strike: 1
intuition: 0
item_id: wode-elf-runner
item_index: '225'
item_name: Wode Elf Runner
level: 1
might: 0
presence: 1
reason: 0
roles:
- Minion Harrier
scc:
- mcdm.monsters.v1:monster:wode-elf-runner
scdc:
- 1.1.1:2:225
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '4'
type: monster
---

~~~ds-statblock
name: Wode Elf Runner
level: 1
roles:
  - Minion Harrier
ancestry:
  - Fey
  - Humanoid
  - Wode Elf
ev: 3 for four minions
stamina: "4"
speed: 7
size: 1M
stability: 0
free_strike: 1
with_captain: Gain an edge on strikes
might: 0
agility: 2
reason: 0
intuition: 0
presence: 1
traits:
  - name: Masking Glamor
    effects:
      - effect: Abilities targeting the runner that would take a bane from cover or
          concealment have a double bane instead.
abilities:
  - name: Spear
    icon: ⚔️
    cost: Signature Ability
    keywords:
      - Charge
      - Melee
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1 or ranged 5
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        t1: 1 damage
        t2: 2 damage
        t3: 3 damage
      - effect: If this ability is used as part of the Charge main action, the runner
          shifts up to 2 squares first
        name: Effect
~~~