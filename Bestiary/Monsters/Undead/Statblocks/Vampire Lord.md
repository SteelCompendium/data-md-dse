---
agility: 5
ancestry:
- Undead
ev: '36'
file_basename: Vampire Lord
file_dpath: Monsters/Undead/Statblocks
free_strike: 7
intuition: 1
item_id: vampire-lord
item_index: '72'
item_name: Vampire Lord
level: 7
might: 2
presence: 2
reason: 1
roles:
- Leader
scc:
- mcdm.monsters.v1:monster:vampire-lord
scdc:
- 1.1.1:2:72
size: 1M
source: mcdm.monsters.v1
speed: 1
stability: 3
stamina: '2200'
type: monster
---

```ds-statblock
name: Vampire Lord
level: 7
roles:
  - Leader
ancestry:
  - Undead
ev: "36"
stamina: "2200"
immunities:
  - Corruption 9
  - poison 9
speed: 1
movement: Climb, hover, teleport
size: 1M
stability: 3
free_strike: 7
might: 2
agility: 5
reason: 1
intuition: 1
presence: 2
traits:
  - name: Lord's Bloodthirst
    effects:
      - effect: The vampire has speed 15 and an edge on power rolls while any creature
          within 20 squares of them is bleeding. Any bleeding creature within 5
          squares of the vampire can't hide.
abilities:
  - name: Crimson Embrace
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature
    effects:
      - roll: Power Roll + 5
        t1: 13 corruption damage; M < 3 bleeding (save ends)
        t2: 21 corruption damage; M < 4 bleeding (save ends)
        t3: 24 corruption damage; M < 5 bleeding (save ends)
      - effect: The vampire regains Stamina equal to half the damage dealt, and can end
          one effect on them that can be ended by a saving throw
        name: Effect
      - effect: The vampire shifts 3 after striking the last target, and can target one
          additional creature for every 2 malice spent.
        cost: 2+ Malice
  - name: Arise, My Children
    cost: 2 Malice
    keywords:
      - Ranged
    type: Maneuver
    distance: Ranged 10
    target: Special
    effects:
      - effect: Two blood-starved vampires appear in unoccupied spaces within distance.
        name: Effect
  - name: Redirected Charm
    cost: 3 Malice
    keywords:
      - Magic
      - Ranged
    type: Free triggered action
    distance: Ranged 5
    target: One enemy
    trigger: A creature makes a strike against the vampire.
    effects:
      - effect: The target becomes the new target of the strike.
        name: Effect
  - name: Let Us Feast!
    cost: Villain Action 1
    keywords:
      - Ranged
    type: "-"
    distance: 20 burst
    target: Each enemy in the area
    effects:
      - effect: Each target who has P < 4 is now bleeding (save ends).
        name: Effect
  - name: Red Mist Rising
    cost: Villain Action 2
    keywords:
      - Area
      - Magic
    type: "-"
    distance: 5 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 5
        t1: 2 damage; M < 3 6 corruption damage
        t2: 7 damage; M < 4 6 corruption damage
        t3: 10 damage; M < 5 6 corruption damage
      - effect: The vampire turns to mist, filling the area. Until the end of the round,
          the vampire can't move or be targeted by abilities, but they can use
          Crimson Embrace against a target in the area. The vampire reforms in
          an unoccupied space in the area at the end of the round.
        name: Effect
```