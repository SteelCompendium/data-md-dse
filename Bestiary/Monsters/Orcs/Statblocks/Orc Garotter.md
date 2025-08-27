---
agility: 2
ancestry:
- Humanoid
- Orc
ev: '6'
file_basename: Orc Garotter
file_dpath: Monsters/Orcs/Statblocks
free_strike: 4
intuition: 1
item_id: orc-garotter
item_index: '135'
item_name: Orc Garotter
level: 1
might: 1
presence: -1
reason: 0
roles:
- Platoon Ambusher
scc:
- mcdm.monsters.v1:monster:orc-garotter
scdc:
- 1.1.1:2:135
size: 1L
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '30'
type: monster
---

```ds-statblock
name: Orc Garotter
level: 1
roles:
  - Platoon Ambusher
ancestry:
  - Humanoid
  - Orc
ev: "6"
stamina: "30"
speed: 5
size: 1L
stability: 0
free_strike: 4
might: 1
agility: 2
reason: 0
intuition: 1
presence: -1
traits:
  - name: Relentless
    effects:
      - effect: If the garroter is reduced to 0 Stamina, they can make a free strike
          before dying. If the target of the free strike is reduced to 0
          Stamina, the garroter is reduced to 1 Stamina instead.
abilities:
  - name: Dagger Feint
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
        t1: 6 damage; the garroter can shift 1 square
        t2: 9 damage; the garroter shifts up to 2 squares
        t3: 12 damage; the garroter shifts up to 3 squares
      - effect: If this ability gains an edge or has a double edge, it deals an extra 4
          damage.
        name: Effect
  - name: Strangle
    icon: 🗡
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature
    effects:
      - roll: Power Roll + 2
        t1: 6 damage
        t2: 9 damage; I < 1 dazed (save ends)
        t3: 12 damage; grabbed; I < 2 dazed (save ends)
      - effect: While grabbed this way, a target can't communicate or use magic
          abilities.
        name: Effect
  - name: Chroma Cloak
    icon: 👤
    cost: 1 Malice
    keywords:
      - "-"
    type: Maneuver
    distance: Melee 1
    target: One creature
    effects:
      - effect: The garroter turns invisible until the end of their turn. This
          invisibility ends early if they take damage or use an ability.
```