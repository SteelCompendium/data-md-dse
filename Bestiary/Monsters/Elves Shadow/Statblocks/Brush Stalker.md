---
agility: 2
ancestry:
- Animal
- Fey
- Shadow Elf
ev: '12'
file_basename: Brush Stalker
file_dpath: Monsters/Elves Shadow/Statblocks
free_strike: 5
intuition: 1
item_id: brush-stalker
item_index: '214'
item_name: Brush Stalker
level: 4
might: 3
presence: 1
reason: -1
roles:
- Platoon Mount
scc:
- mcdm.monsters.v1:monster:brush-stalker
scdc:
- 1.1.1:2:214
size: '2'
source: mcdm.monsters.v1
speed: 8
stability: 3
stamina: '60'
type: monster
---

~~~ds-statblock
name: Brush Stalker
level: 4
roles:
  - Platoon Mount
ancestry:
  - Animal
  - Fey
  - Shadow Elf
ev: "12"
stamina: "60"
speed: 8
size: "2"
stability: 3
free_strike: 5
might: 3
agility: 2
reason: -1
intuition: 1
presence: 1
traits:
  - name: Suneater
    effects:
      - effect: The area within 2 squares of the brush stalker is devoid of light and
          provides concealment.
  - name: Wyrd Dyr
    effects:
      - effect: While they have line of effect to the brush stalker, any animal except
          another brush stalker is frightened
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
    distance: Melee 2
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 3
        t1: 7 damage
        t2: 10 damage
        t3: 13 damage
  - name: Reclamation
    icon: ❇️
    cost: 2 Malice
    keywords:
      - Area
      - Magic
    type: Main action
    distance: 2 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        t1: 4 corruption damage; M < 1 weakened (save ends)
        t2: 7 corruption damage; M < 2 weakened (save ends)
        t3: 10 corruption damage; M < 3 weakened (save ends)
~~~