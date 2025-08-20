---
agility: 2
ancestry:
- Bugbear
- Fey
- Goblin
- Humanoid
ev: '16'
file_basename: Bugbear Sneak
file_dpath: Monsters/Bugbears/Statblocks
free_strike: 5
intuition: 0
item_id: bugbear-sneak
item_index: '288'
item_name: Bugbear Sneak
level: 2
might: 2
presence: 0
reason: 0
roles:
- Elite Ambusher
scc:
- mcdm.monsters.v1:monster:bugbear-sneak
scdc:
- 1.1.1:2:288
size: 1L
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '80'
type: monster
---

```ds-statblock
name: Bugbear Sneak
level: 2
roles:
  - Elite Ambusher
ancestry:
  - Bugbear
  - Fey
  - Goblin
  - Humanoid
ev: "16"
stamina: "80"
speed: 7
size: 1L
stability: 0
free_strike: 5
might: 2
agility: 2
reason: 0
intuition: 0
presence: 0
traits: []
abilities:
  - name: Sucker Punch
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
        t1: 8 damage; A < 1 grabbed
        t2: 13 damage; A < 2 grabbed
        t3: 16 damage; grabbed
      - effect: The target can't use triggered actions until the start of the next
          round. Additionally, if the sneak started their turn hidden from the
          target, this ability deals an extra 4 damage.
  - name: Shadow Cloak
    cost: 3 Malice
    keywords:
      - Area
    type: Main action
    distance: 2 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 2
        t1: 2 damage; I < 0 the sneak has concealment from the target (save ends)
        t2: 3 damage; I < 1 the sneak has concealment from the target (save ends)
        t3: 4 damage; I < 2 the sneak has concealment from the target (save ends)
      - effect: The sneak shifts up to their speed and can attempt to hide.
  - name: Carving Dagger
    keywords:
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Ranged 8
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        t1: 7 damage; M < 0 bleeding (save ends)
        t2: 11 damage; M < 1 bleeding (save ends)
        t3: 14 damage; M < 2 bleeding (save ends)
      - effect: While bleeding this way, the target can't hide from the sneak or their
          allies.
  - name: Throw
    keywords:
      - Melee
      - Strike
    type: Maneuver
    distance: Melee 1
    target: One creature or object
    effects:
      - effect: The target must be grabbed by the sneak.
        name: Special
      - effect: The target is vertical pushed up to 4 squares. An ally doesn't take
          damage from being force moved this way.
  - name: Catcher
    keywords:
      - Melee
    type: Free triggered action
    distance: Melee 1
    target: The triggering creature or object
    trigger: A size 1 creature or object is force moved within distance, or a size 1
      ally willingly moves within distance.
    effects:
      - effect: The target is grabbed by the sneak.
  - name: Clever Trick
    cost: 1 Malice
    keywords:
      - "-"
    type: Triggered action
    distance: Special
    target: One enemy
    trigger: The sneak is targeted by a strike.
    effects:
      - effect: The sneak chooses one enemy within distance of the strike to become the
          target of the strike.
```