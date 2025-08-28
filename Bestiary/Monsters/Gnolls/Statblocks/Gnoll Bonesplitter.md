---
agility: 1
ancestry:
- Abyssal
- Gnoll
ev: '4'
file_basename: Gnoll Bonesplitter
file_dpath: Monsters/Gnolls/Statblocks
free_strike: 3
intuition: 0
item_id: gnoll-bonesplitter
item_index: '39'
item_name: Gnoll Bonesplitter
level: 2
might: 2
presence: 1
reason: 0
roles:
- Horde Brute
scc:
- mcdm.monsters.v1:monster:gnoll-bonesplitter
scdc:
- 1.1.1:2:39
size: 1L
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '25'
type: monster
---

~~~ds-statblock
name: Gnoll Bonesplitter
level: 2
roles:
  - Horde Brute
ancestry:
  - Abyssal
  - Gnoll
ev: "4"
stamina: "25"
speed: 5
size: 1L
stability: 1
free_strike: 3
might: 2
agility: 1
reason: 0
intuition: 0
presence: 1
traits:
  - name: Death Frenzy
    effects:
      - effect: Whenever a non-minion ally within 5 squares of the bonesplitter is
          reduced to 0 Stamina, the bonesplitter moves up to their speed and can
          make a melee free strike.
abilities:
  - name: Three-Tail Flail
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
      - roll: Power Roll + 2
        t1: 5 damage; push 2
        t2: 6 damage; push 2
        t3: 8 damage; grabbed; M < 2 the target takes a bane on the Escape Grab maneuver
      - effect: While the bonesplitter has a target grabbed, they can't use Three-Tail
          Flail against another target.
        name: Effect
  - name: Bonesplitter's Cackletongue
    icon: ❇️
    cost: 4 Malice
    keywords:
      - Area
    type: Maneuver
    distance: 2 burst
    target: Self and each ally in the area
    effects:
      - effect: Up to three targets can make a free strike. If any target hasn't used
          their own Cackletongue maneuver on this turn, they can use it
          immediately at no cost.
        name: Effect
~~~