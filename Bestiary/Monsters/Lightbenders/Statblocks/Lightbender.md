---
agility: 1
ancestry:
- Beast
- Lightbender
ev: '20'
file_basename: Lightbender
file_dpath: Monsters/Lightbenders/Statblocks
free_strike: 6
intuition: 1
item_id: lightbender
item_index: '206'
item_name: Lightbender
level: 3
might: 2
presence: -1
reason: -3
roles:
- Elite Ambusher
scc:
- mcdm.monsters.v1:monster:lightbender
scdc:
- 1.1.1:2:206
size: '2'
source: mcdm.monsters.v1
speed: 1
stability: 1
stamina: '0100'
type: monster
---

```ds-statblock
name: Lightbender
level: 3
roles:
  - Elite Ambusher
ancestry:
  - Beast
  - Lightbender
ev: "20"
stamina: "0100"
speed: 1
size: "2"
stability: 1
free_strike: 6
might: 2
agility: 1
reason: -3
intuition: 1
presence: -1
traits:
  - name: Avoidance
    effects:
      - effect: Any effect on the lightbender that would be ended by a saving throw
          instead ends automatically at the end of their next turn.
abilities:
  - name: Flash Swipe
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 2
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 9 damage
        t2: 14 damage
        t3: 18 damage
      - effect: If this ability gains an edge or has a double edge, it deals an extra 4
          damage.
        name: Effect
  - name: Piercing Tails
    icon: 🗡
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 2
    target: One creature or object
    effects:
      - cost: ≤11
        effect: 8 damage
        t2: 12 damage; M < 1 bleeding (save ends)
        t3: 15 damage; M < 2 bleeding (save ends)
      - effect: While bleeding this way, the target takes a bane on tests to search for
          the lightbender while they are hidden.
        name: Effect
  - name: Hypnotic Mane
    icon: ❇️
    cost: 5 Malice
    keywords:
      - Area
      - Magic
    type: Maneuver
    distance: 3 burst
    target: Each enemy in the area
    effects:
      - cost: ≤11
        effect: I < 0 dazed (save ends)
        t2: I < 1 dazed (save ends)
        t3: I < 2 dazed (save ends)
      - effect: While dazed this way, a target has speed 0. If a target takes damage, or
          if someone else uses a main action to shake the target out of their
          stupor, the dazed condition ends.
        name: Effect
  - name: Stalker's Afterimage
    icon: ❗️
    keywords:
      - Magic
    type: Triggered action
    distance: Self
    target: Self
    trigger: The lightbender takes damage from a strike.
    effects:
      - effect: The lightbender halves the damage, ignores any nondamaging effects
          associated with it, and can teleport up to 5 squares. If they teleport
          into concealment or cover, the lightbender can immediately attempt to
          hide as a free maneuver.
        name: Effect
```