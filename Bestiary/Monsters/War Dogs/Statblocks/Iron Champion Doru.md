---
agility: 4
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '48'
file_basename: Iron Champion Doru
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 0
intuition: 4
item_id: iron-champion-doru
item_index: '377'
item_name: Iron Champion Doru
level: 10
might: 5
presence: 2
reason: 1
roles:
- Elite Brute
scc:
- mcdm.monsters.v1:monster:iron-champion-doru
scdc:
- 1.1.1:2:377
size: 1L
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '2602'
type: monster
---

```ds-statblock
name: Iron Champion Doru
level: 10
roles:
  - Elite Brute
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "48"
stamina: "2602"
speed: 5
size: 1L
stability: 1
free_strike: 0
might: 5
agility: 4
reason: 1
intuition: 4
presence: 2
traits:
  - name: Iron Juggernaut
    effects:
      - effect: Doru can't be made slowed or restrained. Additionally, he can move while
          grabbed, and a creature grabbing him moves along with him unless they
          let go.
  - name: The Scarless
    effects:
      - effect: Doru regains 10 Stamina at the start of each of his turns unless he took
          acid or fire damage since the start of his previous turn. Whe- ever he
          regains Stamina this way, the Director can spend 2 Malice to end one
          effect on Doru that can be ended by a saving throw
  - name: Champion's Loyalty Collar
    effects:
      - effect: When Doru is reduced to 0 Stamina, his loyalty collar explodes, dealing
          20 damage to each enemy and object within 3 squares of him.
abilities:
  - name: Houndaxe
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 2
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 5
        t1: 15 damage
        t2: 21 damage; Doru gains an edge on his next power roll; M < 4 slide 3
        t3: 25 damage; Doru has a double edge on his next power roll; M < 5 slide 5
      - effect: The damage from this ability can't be reduced in any way.
        name: Effect
      - effect: This ability targets one additional target.
        cost: 3 Malice
  - name: Bloody Whirlwind
    cost: 2 Malice
    keywords:
      - Area
      - Weapon
    type: Main action
    distance: Burst 3
    target: Each creature and object in the area
    effects:
      - roll: Power Roll + 5
        t1: 5 damage; A < 3 bleeding (save ends)
        t2: 11 damage; A < 4 bleeding (save ends)
        t3: 15 damage; A < 5 bleeding (save ends)
      - effect: This ability deals an extra 5 damage for each winded target in the area.
        name: Effect
  - name: Hunting Leap
    keywords:
      - Ranged
    type: Maneuver
    distance: Ranged 5
    target: One creature or object
    effects:
      - effect: Doru jumps to an unoccupied space adjacent to the target, then can make
          a free strike against them. If the target is bleeding or winded, the
          distance of the ability becomes Ranged 10 and the free strike deals an
          extra 5 damage.
        name: Effect
  - name: Laugh It Off
    keywords:
      - "-"
    type: Triggered action
    distance: Self
    target: Self
    trigger: An enemy makes a strike against Doru.
    effects:
      - effect: The triggering strike takes a bane and Doru gains an edge on his next
          power roll.
        name: Effect
```